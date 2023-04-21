# egui_phosphor

Bundles Phosphor icons with boilerplate to use in your egui app.

## Installation

Add the crate as a dependency in Cargo.toml:
```toml
egui-phosphor = "0.1.0"
```

On startup, update the fonts in your egui context:
```rust
let mut fonts = egui::FontDefinitions::default();
egui_phosphor::add_to_fonts(&mut fonts);

cc.egui_ctx.set_fonts(fonts);
```

## Usage

Use the constants provided by the crate in your text:
```rust
ui.label(egui::RichText::new(format!("FILE_CODE {}", egui_phosphor::FILE_CODE)).size(32.0));
```