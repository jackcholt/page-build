# page-build
## Fluent interface to building data-injected HTML pages.

This is an exploration of of a more concise way to build HTML web pages.

I consider HTML to be verbose and error-prone for the same reason that XML is verbose and error-prone.  All it takes is to mistype a closing tag, misspell the name of the tag or violate nesting rules.

I have used other approaches to alleviate the problem such as Jade/Pug.  It certainly makes the markup less verbose but it has the downside of introducing a new and proprietary syntax that is not used in any other situation.

This is an attempt to use a Groovy-syntax, fluent interface for constructing HTML web pages into which data can be injected by passing it to the supported methods.

# Example:
pre
new Html5()
.head(title: 'My Awesome Page')
.body(
  id: 'mainPage'
)
