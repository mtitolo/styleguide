.reddit-css {
=============

```
ḃ̭̄̈́̇̐̚͘o̝͈̯̠d̹̜͛̈́̎ͬͨỹ̝̭͛͗ ͕̭̭̣͉͓̓̽̋̄ͦͅ{̲̩͖̤̒
̇ ̦̟ ̪̼͜c͕ͮ̄ŏ̳͓̝͇͕̲͑͂͘l͎̥͇̮̦ͪo͙̜̺̬̫̼͛͊̽ͬ̒̏r͑̈͛:̼̉̍͠ ̤͓͎̖̅͆ͅ#ͪ̄́99͔̤͕͇̙̍̄̍ͩ͑ͦ9̵̒͐̈́ͯͩ̚;̳ͬ͐̆͞
̨̘̲̘͍̰̮ͯ͌̍ͪ̊̅ ̨̦̳͓͇̭̗͕͐̾ͮ͂ͦ̂̃ ̶͆w̳̲̳i̡̻̟͍̮͐̎ͤd͙̱̙̦̋t̖̭̺̦̼̉͡h͊҉̹̗̳̹͚̪:͓̪̖͕ͣ̓̊̇ͯ̄̇ ̯̘͍̀̓1͍͈̟̦̿0̤ͣͮ̋̄0̠̍͗ͣ%͙̓̉̃̓ͧ;̲͕͚̥̟̤͇ͤ̓͒̓̽ͣ
͕̺͎͈̜̼ͧͬ̅͐̅ ̢͙̠͔͋̏ͥ̾ ͋̃̃̀m͔̝̮a͇͈̦͕͔̬̣̒̀r͓͜gͨ̉i͓̼ͣ̂͂́̎n͉̈́ͤ̌̋̏̇ͨ:̗͈̮̲̙̾ͭͫ̓ ̆̇͂ͨ0̤͐̋;̱̫̣͠
̛̝͚ͭͭͯͤ ̴̜͍͕̮͍̍̍ͬ ͇͍̣͖͚̹p͎̍͊̚a̯̪̺̣̮ḓ̣͍̪̝ͅḏ̦̲̥̥̘ͅi̺̬̜͚͓̼̋͆̈́͂ͨ̀n̬̪͙̠͎̲̔̽̚g̗̣̬̭̫͇ͥ͆͆ͅ:̲̥͇̝̬ͣ̈͗͢ͅ ̖̟͚̰̯̣̀́̾ͯ̾̋̓͞ͅ0̉҉̙̫͉;̯̤ͭ͌͞
̣̬̏͛̏̚͞}̬͓͔̜͈ͩ
```

## Coding Style

**Indentation**

Two spaces.

```
.bad-example {
    color: red;
}

.good-example {
  color: #900;
}
```

**Naming**

Names should be descriptive of a discrete component. A selector like `.modal-header`
is a better selector than `.modal > div:first-child > h2`, because it allows us to use
that class in situations where the html structure may not match exactly.

Stay away from ids, which leads you down the dark path of overly specific
styles. Use composable, reusable styles instead. Exceptions include global
elements such as `#header` and `#footer`.

**Specificity**

If you're nesting more than two selectors deep, that's a good indication that
you're being too specific. Consider using more composable styles. For example,
instead of `form.error > .input > label`, use `.error-label` and apply the class
directly. This improves composability and rendering performance.

**Comments**

Use `//` for comments.

**Colors**

Use rgba or hex codes, not colors. If using a CSS preprocessor, such as LESS,
prefer using variables rather than redefining colors.

**Size Units**

Use `px` for `font-size`, because it offers absolute control over text.
Additionally, unit-less `line-height` is preferred because it does not inherit a
percentage value of its parent element, but instead is based on a multiplier of
the `font-size`.

> Ed. note: we may investigate use of `rem`s.

}
=
