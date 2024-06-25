---
title: A Taste Of TUIs
author: Troels Hoffmeyer
theme:
  # Specify it by name for built-in themes
  name: dark
---

Who Am I
---
![ignored](assets/Beosound_A5.png)
 * Engineer at Bang & Olufsen
 * Rustacean since 2019 (I think)
<!-- end_slide -->
What is this talk about
---
![ignored](assets/dtui.png)
<!-- end_slide -->
What do i hope you get from this talk
---

- A small look at how to do a TUI in Ratatui
- A dip in the pool of dbus and how to use the zbus crate
<!-- end_slide -->
Ratatui
---

![ignored](assets/ratatui-logo.png)

 * https://ratatui.rs/
<!-- end_slide -->
---
 * Easily create powerful Terminal UIs
 * Compatible with multiple backend libraries (crossterm, termion, termwiz)
 * Comes with a bunch of prebuilt "widgets" like Gauges, Charts, List...
 * Fork and replacement for tui-rs, now community maintained and really successful
<!-- end_slide -->

Demo
---
![ignored](assets/demo2.gif)
<!-- end_slide -->

Bottom
---
![ignored](assets/bottom-demo.png)
<!-- end_slide -->
Scope TUI
---
![ignored](assets/scope-tui.png)
<!-- end_slide -->
Raffle
---
![ignored](assets/raffle.png)
<!-- end_slide -->
zbus
---

 * https://dbus2.github.io/zbus/
<!-- end_slide -->
The App
---
```rust
pub struct App {
    dbus_rx: Receiver<AppMessage>,
    dbus_handle: DbusActorHandle,
    pub services: StatefulList<OwnedBusName>,
    pub objects: StatefulTree,
    pub working_area: WorkingArea,
}
```
<!-- end_slide -->
---
## Thank you Alice

![ignored](assets/made_a_mistake.png)
<!-- end_slide -->