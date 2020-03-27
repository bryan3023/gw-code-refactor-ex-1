# gw-homework01
## Synopsis
This project is the deliverable for **01 HTML CSS Git: Code Refactor**. The overall goals were:

* Refactor and clean up the HTML code, using semantic tags where possible.
* Clean up the CSS code, looking for opportunities to simplfy and considate the code.
* Provide alt text content for all images to enhance accessibility.
* Give the page a more meaningful title.
* Ensure all links work.

## Change Notes
### index.html
* Updated the title to make it more meaningful.

* Changed `<div class="header">` to `<header>`.

* Changed the `<div>` within `<header>` to `<nav>`.

* Changed `<div class="hero">` to `<div class="hero-image">` to make it a bit more [self-documenting](https://en.wikipedia.org/wiki/Self-documenting_code). I didn't see a semantic tag that would be appropriate in this case.

* Changed `<div class="content">` to `<main>`.

* Added `id="search-engine-optimization"` to the first `<div>` under `<main>` to fix the broken link from the navigation menu.

* Under `<main>`, changed all `<div>`s to `<section>`s. Also removed the `class` attributes from all `<section>`s, as these were redundant with the `id`s.

* Changed `<div class="benefits">` to `<aside>`.

* Under `<aside>`, changed all `<div>`s to `<section>`s. Removed the `class` attribute from all `<section>`s.

* Within `<aside>`'s last `<section>`, changed `<img></img>` to `<img />`.

* Changed `<div class="footer">` to `<footer>`.

* Added descriptive `alt` text to all `<img>`s.

### style.css
* Re-organized the CSS to make it a bit easier to follow. Put document-wide properties at the top and then reordered the rest to match the document flow.

* Updated CSS selectors to match tag changes in HTML file.

* Consolidated several redundant CSS selectors. For example, within both `main` and `aside`, their `section`s were uniform, so there was no need for the `class`/`id`-specific selectors.