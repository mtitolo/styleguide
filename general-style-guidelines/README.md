# reddit General Style Guidelines

Check out the [reddit/reddit wiki](https://github.com/reddit/reddit/wiki) for
additional resources.

## The Golden Rule

Follow the style of the file you're in. It's more important to be *contextually*
correct than it is to be *absolutely* correct.

## "Reddit"

reddit is always lowercase, even at the start of sentences. Many headings and messages around the site are stylistically lowercased as well.

## Git workflow

### Commits

Individual commits should be atomic changes to the codebase. Specifically:

* A commit should not leave the code in a broken state waiting on a later
  commit to fix it.
* Changes that aren't related should be split into separate commits. This
  must be taken with the previous rule in mind to help determine what's
  related or not.  Bugfixes that are prerequisites to your change but not
  the main point of the change should be made in separate commits that come
  first.


### Commit Messages

Follow the [git commit message standard](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html):

```
Capitalized, short (50 chars or less) summary

More detailed explanatory text, if necessary.  Wrap it to about 72
characters or so.  In some contexts, the first line is treated as the
subject of an email and the rest of the text as the body.  The blank
line separating the summary from the body is critical (unless you omit
the body entirely); tools like rebase can get confused if you run the
two together.

Write your commit message in the imperative: "Fix bug" and not "Fixed bug"
or "Fixes bug."  This convention matches up with commit messages generated
by commands like git merge and git revert.

Further paragraphs come after blank lines.

- Bullet points are okay, too

- Typically a hyphen or asterisk is used for the bullet, preceded by a
  single space, with blank lines in between, but conventions vary here

- Use a hanging indent


```

Prefixing the commit message summary with the subsystem being affected
can be helpful sometimes, e.g. `/dev/api: Document subreddit endpoints.`.

It's a good idea to include the rationale for a change in the explanatory
text for non-trivial changes.  When in doubt, think about what would be
useful three years down the line when blaming a weird line of code.

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
