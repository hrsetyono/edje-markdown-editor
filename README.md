# hEditor

![H Editor](https://raw.github.com/hrsetyono/cdn/master/edje-js/h-editor-1.1.png)

A StackOverflow-style interface for using Markdown with textareas.

- **Pure JavaScript** - No jQuery or other library.

- **Lightweight** - Only 5.3 KB gzipped.

- **100% Compatible** - It's still a plain textarea, so no need to worry about lag or crashing on mobile.

| Demo | Link |
| --- | --- |
| Basic Usage | [View in Codepen](https://codepen.io/hrsetyono/pen/PoPXXNq) |

## How to Use

First, get the CSS and JS file from `/dist` folder.

Then use this function to initiate the editor:

```js
hEditor( textarea, [args] )
```

`textarea` (Node) - The textarea that you want to add buttons to.

`args` (Object / optional)

- **`buttons`** (array) - Specify the order of buttons.

    Default: `[ 'bold', 'italic', 'link', '|', 'bullist', 'numlist', 'image', 'quote' ],`

    Pipe symbol (`|`) means separator.

    Other available buttons: `h1`, `h2`, `h3`, `code`, `pre`, `hr`, `strike`, `undo`, `redo`


## Example

```js
<textarea id="comment"></textarea>

<script>
document.addEventListener('DOMContentLoaded', () => {
  'use strict';

  hEditor( document.querySelector( '#comment' ), {
    buttons: [ 'bold', 'italic', 'link', '|', 'bullist', 'numlist', 'image', 'quote' ],
  } );
});
</script>
```

## Known Bugs

- In Firefox, you can't undo the tag insertion. This is due to this [Firefox bug](https://bugzilla.mozilla.org/show_bug.cgi?id=1220696)

## Credit

This is a fork of [MarkdownEditor](https://github.com/hrsetyono/MarkdownEditor) with added features like List and Inline Code. So big thanks to [Digital Nature](https://github.com/digitalnature) for creating an awesome basis for this library.