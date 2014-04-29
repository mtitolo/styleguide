# reddit General Style Guidelines

Check out the [reddit/reddit wiki](https://github.com/reddit/reddit/wiki) for
additional resources.

## The Golden Rule

Follow the style of the file you're in. It's more important to be *contextually*
correct than it is to be *absolutely* correct.

## "Reddit"

reddit is always lowercase, even at the start of sentences. Many headings and messages around the site are stylistically lowercased as well.

## Git workflow

### Use verbose, topical branches.

```
# bad:
$ git checkout -b fix-js-bug

# good:
$ git checkout -b fix-js-error-on-expanding-image-galleries
```

Similarily, use verbose, topical commits. Stick to 80 characters, and add
verbose commit messages if necessary. Use capitalization and punctuation.

### Make sure changes are rebased on latest master.

Ensure your code is up-to-date to prevent merge conflicts and make testing
easier.

