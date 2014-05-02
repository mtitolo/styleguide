# reddit Android style guidelines

## General Style

In general, reddit tries to follow the
[Android code style](https://source.android.com/source/code-style.html)
guidelines. We're still iterating quickly and learning,
so we often fall short, but the expectation is for improvements
to happen over time.

## Listen to Your Tools

Android Studio is our IDE, and it provides all sorts of
useful features. Don't add code that causes IDE or compiler
warnings. If necessary, use the `@SuppressWarnings` annotation
\- but only if you are certain that is the best approach.

## Short term rule: Be INCONSISTENT

Our Android codebase is new. Existing code may not follow
the guidelines. Don't try to be "consistent" with the existing
code - write new code that follows the guidelines, and fix old
code to also follow the guidelines.

