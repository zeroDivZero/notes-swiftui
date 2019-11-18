# PREVIEWS

Can apply modifiers to main content view in previews section. Can show multiple previews at same time.

```swift
struct ContentView_Previews: PreviewProvider {
    static var previews: some View {
        Group {
            ContentView()
            ContentView()
                .colorScheme(.dark)
                .background(Color.black)
                .previewDevice("iPad Pro (9.7-inch)")
        }
    }
}
```

Opt-click `previewDevice()` for possible devices.
