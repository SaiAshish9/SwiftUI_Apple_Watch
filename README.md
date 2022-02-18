```
Slider(value: Binding(get: {
  self.value
}, set: {(newValue) in
  self.value = newValue
  self.update()
}), in: 1...4, step: 1)
  .accentColor(.accentColor)
```

```
 HStack {
  Capsule()
    .frame(height: 1)
  
  Image(systemName: "note.text")
  
  Capsule()
    .frame(height: 1)
} //: HSTACK
.foregroundColor(.accentColor)
```

```
import Foundation

struct Note: Identifiable, Codable {
  let id: UUID
  let text: String
}

```
