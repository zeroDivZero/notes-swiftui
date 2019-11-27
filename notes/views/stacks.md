# STACKS

`View`'s `body` returns 1 `View`. Use stack to arrange multiple child views in major axis.

3 types: `VStack`, `HStack`, `ZStack`.

## VStack

Arranges children in vertical line.

```swift
VStack {
    Text("Huli Pizza")
    Text("Order pizza")
}
```

## HStack

Arranges children in horizontal line.

```swift
HStack {
    Text("Chicken pizza")
    Image("chicken_pizza")
    Spacer()
    Text("2x")
    Text("$15.00")
    Text("=")
    Text("$30.00")
}
```

## ZStack

Arranges children from back to front.

```swift
ZStack {
    Image("surfboard")
    Text("Huli Pizza")
}
```

## Alignment and Spacing

For `VStack` and `HStack`, can optionally specify `alignment` and `spacing` (between adjacent children; if `nil`, use default). For `ZStack`, can specify `alignment`.

```swift
VStack(alignment: .trailing) { // horizontal alignment
  ...
}

HStack(alignment: .firstTextBaseline, spacing: 15.0) { // vertical alignment
  ...
}

ZStack(alignment: .topLeading) {
  ...
}
```
