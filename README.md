# hEditor

A StackOverflow-style interface for using Markdown with textareas.

- Require jQuery (pure JS will come soon)

- Only 3.8KB gzipped

![H Editor](https://raw.github.com/hrsetyono/cdn/master/edje-js/h-editor.png)

## Demo

| Name | Link |
| --- | --- |
| Basic Usage | [View in Codepen](https://codepen.io/hrsetyono/pen/PoPXXNq) |

## How to Use

```js
$( 'textarea' ).hEditor({
  tools: [ 'bold', 'italic', 'link', '|', 'bullist', 'numlist', 'quote', '|', 'image', 'code', 'pre' ],
});
```

**ARGUMENTS**

- **`tools`** (array) - Specify the order of buttons. The example above already include all supported buttons.


### Known Bugs

- In Firefox, you can't undo the tag insertion. This is due to this [Firefox bug](https://bugzilla.mozilla.org/show_bug.cgi?id=1220696)

### Credit

This is a fork of [MarkdownEditor](https://github.com/hrsetyono/MarkdownEditor) with added features like List and Inline Code. So big thanks to [Digital Nature](https://github.com/digitalnature) for creating an awesome basis for this library.