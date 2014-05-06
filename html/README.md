`<!DOCTYPE html>`
=================

*An html style guide to turn that :&lt; into a :>*

## Document Guidelines

### Doctype

Use the `html5` doctype at all times at the top of your html document:
`<!DOCTYPE html>`.

### `<html>`

Add a `lang` attribute to your `<html>` tag.

### `<head>`

* Always include a title tag.
* Include `<meta>` tags for `keywords` and `description` on search-engine-friendly pages.
* Include a favicon.
* Use IE conditional comments to load IE-specific stylesheets.
* Load as few stylesheets as prudent.
* Don't load javascript files in the head unless absolutely necessary.

### `<body>`

* Optionally include a class on body descriptive of the current page.
* Load javascript at the bottom.
* Use the most specific element possible; `ol` for odered lists, `a` for links, `button` for buttons.
  Use appropriate html5 structure elements, such as `aside` and `article`.

### `<form>`

* Every form input should have a `<label>` tag, *especially radio and checkbox elements*.

## Style

* 2 space indentation.
* Always use quotes for attributes.
* Use "double quotes" for attributes.
* `html5` allows the skipping of closing tags (the `/` in `<br />`); do so consistently.
* CSS classes should be lowercase, hyphenated, and descriptive. `.upvote-arrow-active`, not `.upvoted`.

## Template Guidelines

* Use minimal logic in templates.
* Keep html in templates, rather than controllers.
* Make sure all text is i18n'd.
