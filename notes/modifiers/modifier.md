# MODIFIER

Attribute to be applied to `View`. Many types: `Controls`, `Effect`, `Layout`, `Text`, `Image`, `List`, etc. Can drag from library to canvas or code. Represented as function that returns modified view.

```swift
Image("Surf Board")
    .resizable()
    .scaledToFit()
```

Order matters: If `resizable()` and `scaledToFit()` swapped, image won't resize.
