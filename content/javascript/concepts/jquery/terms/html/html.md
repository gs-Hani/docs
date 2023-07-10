---
Title: '.html()'
Description: 'Gets or sets the contents of an HTML element.'
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

The **`.html()`** method gets or sets the contents of an [HTML element](https://www.codecademy.com/resources/docs/html/elements).

## Syntax

Getting HTML, the `.html()` method is called without a parameter:

```pseudo
$(selector).html();
```

Setting HTML, the `.html()` method is called with a parameter containing the new HTML:

```pseudo
$(selector).html(newHTML)
```

## Example

The following jQuery code will read and reset the HTML in `#p1` when `#btn` is clicked:

<!-- prettier-ignore -->
```js
$("#btn").click(function() {
  alert($("#p1").html());
  $("#p1").html("<b>New Text.</b>");
});
```
## Codebyte Example

The following jQuery code will convert the HTML in `#p` to text when clicked:

```codebyte/html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>html demo</title>
    <style>
    p      { margin: 8px; font-size: 20px; color: blue; cursor: pointer; }
    b      { text-decoration: underline; }
    button { cursor: pointer; }
    </style>
    <script src="https://code.jquery.com/jquery-3.7.0.js"></script>
  </head>
  <body>
  
    <p>
      <b>Click</b> to change the <span id="tag">html</span>
    </p>
    <p>
      to a <span id="text">text</span> node.
    </p>
    <p>
      This <button name="nada">button</button> does nothing.
    </p>
    
    <script>
      $( "p" ).on( "click", function() {
        const htmlString = $( this ).html();
        $( this ).text( htmlString );
      });
    </script>
  
  </body>
</html>
```