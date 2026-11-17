# Nero Client (Fabric)

Features: FPS Boost, Fullbright, Underground mob ESP. Open the menu in game with `/nero`.

- The ESP only runs underground and only highlights mobs, never players.
- FPS Boost saves your current video settings and restores them when you turn it off.

## Build

1. Install JDK 21 for the 1.21.11 folder, or JDK 25 for the 26.2 folder.
2. In the folder, run `gradle wrapper` once (or open it in IntelliJ and let it import), then `./gradlew build`.
3. The jar is in `build/libs/` (use the one without `-sources`). Put it in your `mods` folder with Fabric API.

## Check before building

- I could not compile this here, so the first build may need small fixes if Mojang renamed an API.
- 1.21.11: confirm loader and Loom versions at https://fabricmc.net/develop/.
- 26.2: `loader_version` and `fabric_api_version` in `gradle.properties` are placeholders you must fill in.
