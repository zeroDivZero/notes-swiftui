# VIEW

Most declarative UI frameworks aim to boil UI down to components, to be combined and composed to form complex views, animations, and interactions.

In SwiftUI, component is view, defined by protocol `View`, which has single property `body`, which is `View`. Recursive design allows views to be embedded in other views.

With new _DSL-like_ syntax (omits `return`) and keywords, can use protocol with associated type as return type.

```swift
struct WelcomeView: View {
    var body: some View {
        Text("Welcome to my fantastic app!")
    }
}
```
