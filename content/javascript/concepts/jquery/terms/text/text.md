---
Title: '.text()'
Description: 'Gets or sets the text of an HTML element.'
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

The **`.text()`** method gets or sets the text of an [HTML element](https://www.codecademy.com/resources/docs/html/elements).

## Syntax

Getting text, the `.text()` method is called without a parameter:

```pseudo
$(selector).text();
```

Setting text, the `.text()` method is called with a parameter containing the new text:

```pseudo
$(selector).text(newtext)
```

## Example

The following jQuery code will read and reset the text in `#p1` when `#btn` is clicked:

<!-- prettier-ignore -->
```js
$("#btn").click(function() {
  alert($("#p1").text());
  $("#p1").text("New Text.");
});
```
## Codebyte Example

The following jQuery code will find the text in the first paragraph (stripping out the html), then set the html of the last paragraph to show it is just text (the red bold is gone).

```codebyte/html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>text demo</title>
  <style>
  p {
    color: blue;
    margin: 8px;
  }
  b {
    color: red;
  }
  </style>
  <script src="https://code.jquery.com/jquery-3.7.0.js"></script>
</head>
<body>
 
<p><b>Test</b> Paragraph.</p>
<p></p>
 
<script>
const str = $( "p" ).first().text();
$( "p" ).last().html( str );
</script>
 
</body>
</html>
```