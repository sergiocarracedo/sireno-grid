CHANGELOG

0.2.1 2018-11-11
================

- Change gutter with to 16px
- Add new breakpoint *lxs* (landscape xs) (min width: 576px)
- Add .col-*#{$breakpoint}*-end-*#{$i}* class that allow to choose **col** end (NOTE: no .col-*#{$breakpoint}*-start-*#{$i}* )
- Gutters change to margin
- Gutters follow same philosophy as col-*#{$breakpoint}*, applies to upper breakpoints.
- Rename .no-*#{$breakpoint}*-gutters to .no-gutters-*#{$breakpoint}*, .no-*#{$breakpoint}*-gutter-left to .no-gutter-left-*#{$breakpoint}* and .no-*#{$breakpoint}*-gutter-right to .no-gutter-right-*#{$breakpoint}*
- Add .gutter-left-*#{$breakpoint}* and  .gutter-right-*#{$breakpoint}*
