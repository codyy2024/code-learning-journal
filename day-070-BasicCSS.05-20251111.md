# Day 70: Basic CSS - CSS Combinators?

## Key topics covered:
- [x] sdf sd

CSS combinators are used to select elements based on their relationship to other elements, and applies more precise and efficient styling.
- (all) descendant combinator ` ` (space)
  > Example: `figure img` in a .css file will style **all** `img` "children" (or grand-children if any) elements under the "parent" `figure`
- (direct) child combinator `>`
  > Example: `figure > img` in a .css file will style **only** the immediate `img` "child" element after the "parent" `figure`
- next-sibling combinator `+`
  > Example: `img + figcaption` in a .css file will style **only** the immediate `figcaption` "sibling" element after the "elder sister" `img`
- subsequent-sibling combinator `~`
  > Example: `img ~ figcaption` in a .css file will style **all** the `figcaption` "sibling" elements after the "elder sister" `img`

