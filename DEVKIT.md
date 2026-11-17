# Rojo for the Roblox Devkit

A fork of [Rojo](https://github.com/rojo-rbx/rojo) 7.7.1 for the Roblox Devkit, kept only until Rojo
releases the same change. Each change is its own commit on the `devkit` branch:

- **The plugin connects when a marker asks,** from [rojo-rbx/rojo#1326](https://github.com/rojo-rbx/rojo/pull/1326)'s
  plugin half, so an agent can connect without a click. On top of it, the plugin keeps listening after
  the first marker, and accepts the session a marker names without confirmation, unless the project's
  `servePlaceIds` leave this place out.
- **The plugin looks for updates among this fork's releases,** not Rojo's: Rojo counts the version's suffix as a
  prerelease, so it would announce Rojo's own 7.7.1 as newer.
- **The version is `7.7.1-devkit.3`,** and the release workflow doesn't upload the plugin to Roblox.

`rojo serve` is unchanged. `7.7.1-devkit.1` also carried
[rojo-rbx/rojo#1350](https://github.com/rojo-rbx/rojo/pull/1350)'s crash fix, dropped because a folder
removed and restored by a branch switch was then never watched again.

Rojo is licensed under the Mozilla Public License 2.0; see [LICENSE.txt](LICENSE.txt).
