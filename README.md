# AppleSkin (Horizon native mod)

A port of [AppleSkin](https://github.com/squeek502/AppleSkin): the hidden parts of hunger, drawn over the food bar as the original does:

- **Saturation icons** over the food icons: how much saturation you have, in the original's four frames.
- **Held food preview**: while you hold food, the food it would restore appears as drumsticks, and the health natural regeneration would give back shows as hearts. Both are dimmed. The animation is set in Settings > Animation: fade (the held food fades in and out), pulse (it breathes while shown), or fade + pulse (it fades in, then pulses, then fades out). Fade + pulse is the default. Faint hearts also show the health you would have if eating restored all of it. When your food is full, the saturation the food would add appears as yellow saturation icons.

## Install

Build it from the command line, or from the launcher window (Settings → Game → Native mods (experimental)) once it is in the registry. The launcher downloads its own Rust and builds the game with your native mods; see Horizon's [native mods](https://github.com/horizon-rust/horizon/blob/main/docs/native-mods.md).

## Build and test

```sh
cargo +stable test
horizon-launcher native-build mixins/appleskin --trust-native-code
```

License: Unlicense (public domain), the same as the original AppleSkin by squeek.
