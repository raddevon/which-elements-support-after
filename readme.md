#Which Elements Support :after?

This page generates a not necessarily comprehensive list of elements that support the :after pseudo-element. It was inspired by a recent problem I had trying to style `hr` with an `:after` pseudo-element. Oddly, this worked when I styled with the most basic element selector (`hr`), but failed when I tried to limit this any at all (`div > hr`).

It works by containing an empty element of most of the HTML 5 elements and using an actual `:after` pseudo-element to display a message indicating support for the element. Each element's tag name is inserted into an attribute with jQuery. The contents of this tag along with the message are then used as the content of the `:after` pseudo-element. As a result, this page is somewhat ugly. Many of the messages have taken on some default styling of their parent elements.

Notable elements without `:after` support:
* `hr`
* form `input` elements and `textarea`
* `select` fields