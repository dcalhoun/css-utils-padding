# css-utils-padding
[![Build Status](https://travis-ci.org/dcalhoun/css-utils-padding.svg?branch=master)](https://travis-ci.org/dcalhoun/css-utils-padding)

Immutable, CSS padding utilities.

## Naming Convention
Due to the ubiquitous nature of setting padding, these utilities use a shorthand
naming convention.

| Shorthand | Description                |
| --------- | -----------                |
| p         | Padding                    |
| t         | Top                        |
| r         | Right                      |
| b         | Bottom                     |
| l         | Left                       |
| x         | XAxis (left and right)     |
| y         | YAxis (top and bottom)     |
| 0         | 0 reset                    |
| 1         | --space-1 (default 0.5rem) |
| 2         | --space-2 (default 1rem)   |
| 3         | --space-3 (default 2rem)   |
| 4         | --space-4 (default 4rem)   |

Change or reset default paddings using the white space scale. Negative u-xAxis
paddings are used to offset paddings and padding of child elements. Padding
auto is used to horizontally center block-level elements with a set width.

```css
.u-p0  { padding:        0 }
.u-pt0 { padding-top:    0 }
.u-pr0 { padding-right:  0 }
.u-pb0 { padding-bottom: 0 }
.u-pl0 { padding-left:   0 }
.u-px0 { padding-left:   0; padding-right:  0 }
.u-py0 { padding-top:    0; padding-bottom: 0 }

.u-p1  { padding:        var(--space-1) }
.u-pt1 { padding-top:    var(--space-1) }
.u-pr1 { padding-right:  var(--space-1) }
.u-pb1 { padding-bottom: var(--space-1) }
.u-pl1 { padding-left:   var(--space-1) }
.u-px1 { padding-left:   var(--space-1); padding-right:  var(--space-1) }
.u-py1 { padding-top:    var(--space-1); padding-bottom: var(--space-1) }

.u-p2  { padding:        var(--space-2) }
.u-pt2 { padding-top:    var(--space-2) }
.u-pr2 { padding-right:  var(--space-2) }
.u-pb2 { padding-bottom: var(--space-2) }
.u-pl2 { padding-left:   var(--space-2) }
.u-px2 { padding-left:   var(--space-2); padding-right:  var(--space-2) }
.u-py2 { padding-top:    var(--space-2); padding-bottom: var(--space-2) }

.u-p3  { padding:        var(--space-3) }
.u-pt3 { padding-top:    var(--space-3) }
.u-pr3 { padding-right:  var(--space-3) }
.u-pb3 { padding-bottom: var(--space-3) }
.u-pl3 { padding-left:   var(--space-3) }
.u-px3 { padding-left:   var(--space-3); padding-right:  var(--space-3) }
.u-py3 { padding-top:    var(--space-3); padding-bottom: var(--space-3) }

.u-p4  { padding:        var(--space-4) }
.u-pt4 { padding-top:    var(--space-4) }
.u-pr4 { padding-right:  var(--space-4) }
.u-pb4 { padding-bottom: var(--space-4) }
.u-pl4 { padding-left:   var(--space-4) }
.u-px4 { padding-left:   var(--space-4); padding-right:  var(--space-4) }
.u-py4 { padding-top:    var(--space-4); padding-bottom: var(--space-4) }

.u-pxn1 { padding-left: -var(--space-1); padding-right: -var(--space-1); }
.u-pxn2 { padding-left: -var(--space-2); padding-right: -var(--space-2); }
.u-pxn3 { padding-left: -var(--space-3); padding-right: -var(--space-3); }
.u-pxn4 { padding-left: -var(--space-4); padding-right: -var(--space-4); }

.u-plAuto { padding-left: auto }
.u-prAuto { padding-right: auto }
.u-pxAuto { padding-left: auto; padding-right: auto; }
```

## Credits
This utility is heavily inspired by [Basscss](http://www.basscss.com) and
[SuitCSS](http://suitcss.github.io). This repository is merely a combining of
great principles championed by each.
