# configure

Overrides the current bar configuration

```
type BarComponent {
    name: String,
//                                   text   | [text, fg_color, bg_color]
    render: (monitor_id: Number) -> (String | [String, Number, Number])[],
    font: String?,
    color: Number?,
}
```

```
type BarSettings {
    height: Number?,
    font_size: Number?,
    font: String?,
    color: Number?,
    components: {
        left: BarComponent[],
        center: BarComponent[],
        right: BarComponent[]
    }
}
```
## Signature

```nogscript
fn configure(settings: BarSettings) -> Void
```

