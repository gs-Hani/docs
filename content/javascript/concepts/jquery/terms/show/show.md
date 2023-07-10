---
Title: '.show()'
Description: 'Shows a hidden HTML element.'
Subjects:
  - 'Web Development'
  - 'Computer Science'
Tags:
  - 'DOM'
  - 'Events'
  - 'Functions'
  - 'jQuery'
  - 'Methods'
CatalogContent:
  - 'introduction-to-javascript'
  - 'paths/full-stack-engineer-career-path'
---

The **`.show()`** method shows a hidden [HTML element](https://www.codecademy.com/resources/docs/html/elements).

## Syntax

```pseudo
$(selector).show(speed, callback);
```

- `selector`: Specifies the elements that will be shown.
- `speed`(optional): Can be "slow" or "fast" or the number of milliseconds.
- `callback`(optional): A [function](https://www.codecademy.com/resources/docs/javascript/callbacks) that is called once the element is displayed.

## Example

The following jQuery code will show the element selected with `#hide` when the `#show` element is clicked:

<!-- prettier-ignore -->
```js
$("#show").click(function() {
  $("#hide").show();
});
```
## Codebyte Example

The following jQuery code will animates all hidden paragraphs to show slowly, completing the animation within 600 milliseconds.

```codebyte/html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>show demo</title>
  <style>
  p {
    background: yellow;
  }
  </style>
  <script src="https://code.jquery.com/jquery-3.7.0.js"></script>
</head>
<body>
 
<button>Show it</button>
<p style="display: none">Hello  2</p>
 
<script>
$( "button" ).on( "click", function() {
  $( "p" ).show( "slow" );
});
</script>
 
</body>
</html>
```