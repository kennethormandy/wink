# Changelog
<div id="changes" data-magellan-destination="changes"></div>

All the latest and greatest changes to Ink.

***

## Wink v0.x.x – Initial Fork

<div id="v0-2-0"></div>
###### v0.2.0

* Adds `.knockout` helper and docs
* Adds `.left` helper
* Adds `.right` helper
* Adds receipt template
* Adds breakout template

<div id="v0-1-0"></div>
###### v0.1.0

* Moves documentation to Markdown
* Moves examples and test to EJS with [Harp](http://harpjs.com), dropping PHP dependency
* Cleans up CSS as SCSS
* Improves typographic scale (more to come)
* Adds fonts, and improves font stacks
* Reduces colors and makes them variables
* Removes button borders on hover
* Improves `.panel` so it’s more like a block-level `<a>`

## Ink v1.0.x – Public Release

<div id="v1-0-5"></div>
###### v1.0.5

* Add `.sub-grid` class to enable the use of sub-grids with panels
* Add paragraph `.lede` class
* Lower specificity on `.panel` class to allw its use on <kbd>&lt;div&gt;</kbd>s
* Partially patch docs examples to work in Firefox
* Normalize font rendering in <kbd>&lt;td&gt;</kbd>s for Outlook 2007/2010/2013
* Fix 100% width issue on iPad
* Remove offset-sub-columns
* Remove proprietary <kbd>&lt;unsubscribe&gt;</kbd> tags from templates
* Fix issue with `.one.sub-columns` sections
* Expand the Getting Started section of the docs
* Add full-width row example to the docs
* Add offset-columns example to the docs
* Add additional panel examples to the docs
* Miscellaneous bug fixes and typo fixes

<div id="v1-0-4"></div>
###### v1.0.4

* Apply font styles more uniformly to fix clients that strip out the <kbd>&lt;body&gt;</kbd> tag (fixes inliner preview)
* Remove percentage based padding on sub-grid (fixes Outlook 2000/2002/2003)
* Add Bower package metadata
* Remove min-width for <kbd>&lt;center&gt;</kbd> tags nested under the sub-grid
* Add helper aliases to `.text-pad` classes (ex. `.left-text-pad` can now be called using `.text-pad-left`)
* Fix `.text-pad` classes nested under aliased `.column` tables
* Remove deprecated button syntax
* Fix link color in headings for Outlook 2007/2010/2013

<div id="v1-0-3"></div>
###### v1.0.3

* Add text-pad classes
* Lower heading sizes to more reasonable defaults
* Add compatibility chart of supported/tested clients to the docs

<div id="v1-0-2"></div>
###### v1.0.2

* Switch to new button syntax to fully support Microsoft Outlook
* Add changelog to Docs

<div id="v1-0-1"></div>
###### v1.0.1

* Fix crushed-image issue in Gmail (mobile, Android, iOS) by adding a min-width to <kbd>&lt;center&gt;</kbd> tags

<div id="v1-0-0"></div>
###### v1.0.0

* Initial Launch
* Grid
* Sub-Grid
* Block-Grid
* Buttons
* Panels
* Retina Images
