# Day 69: Basic CSS -  `width`, `height`

## Key topics covered:
- [x] `width`, `height`, `min-width`, `min-height`, `max-width`, and `max-height`

## 1. `width`, `height`
In CSS, the width and height properties are used to control the dimensions of elements on a webpage. They can be in different measusing units:
- pixels `px`
- percentage `%`
- viewport units `vw` and `vh`
- and more

## 1.1 If not specified, it's set to `auto` 
- div `width: auto` makes it expand to fill the full width of its parent container
- `width: height` means it will adjust to the content inside.

## 1.2 `min-width`, `min-height`, `max-width`, and `max-height`
They will override the  `width`, `height`.

This will be a box of 100px x 100px
```
<head>
  <style>
    .box {
      width: 50px;
      min-width: 100px;
      height: 50px;
      min-height: 100px;
      background-color: lightcoral;
    }
  </style>
</head>
<body>
  <div class="box"></div>
</body>
```

This will be a box of 150px x 150px
```
<head>
  <style>
    .box {
      width: 200px;
      max-width: 150px;
      height: 200px;
      max-height: 150px;
      background-color: lightgreen;
    }
  </style>
</head>
<body>
  <div class="box"></div>
</body>
```

## Suggestions
1. The whole explanation in this episode is a bit all over the place and repetitive - make it short, precise and clutter-free.

[Ends 08:58 10 Nov 2025]
