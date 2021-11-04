# Sass @mixin and @include

## dynamic sass for position-absolute

```
@mixin position-absolute($top: null, $left: null, $right: null, $bottom: null) {
    position: absolute;
    top: $top;
    left: $left;
    right: $right;
    bottom: $bottom;
}
```

## dynamic sass for background image

```
@mixin bgImage($image) {
    background: url($image);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-blend-mode: overlay;
}
```

### include

```
@include bgImage("/images/1.jpg");
```

## FlexBox 

```
@mixin flexCenter {
    display: flex;
    align-items: center;
    justify-content: center;
}
```
```
@mixin flexSpace {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```
```
@mixin flexVertical {
    display: flex;
    align-items: center;
}
```

### include

```
@include flexCenter;
@include flexSpace;
@include flexVertical;

```
