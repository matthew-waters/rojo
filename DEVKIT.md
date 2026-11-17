# Rojo for the Roblox Devkit

A fork of [Rojo](https://github.com/rojo-rbx/rojo) 7.7.1 for the Roblox Devkit, kept only until Rojo
releases the same changes. Each change is its own commit on the `devkit` branch:

- **The plugin connects when a marker asks,** from [rojo-rbx/rojo#1326](https://github.com/rojo-rbx/rojo/pull/1326)'s
  plugin half, so an agent can connect without a click. It keeps listening after the first marker, and
  accepts a session the marker names without confirmation.
- **`rojo serve` doesn't crash when a changed path no longer exists,** from
  [rojo-rbx/rojo#1350](https://github.com/rojo-rbx/rojo/pull/1350).
- **The version is `7.7.1-devkit.1`,** and the release workflow doesn't upload the plugin to Roblox.

Rojo is licensed under the Mozilla Public License 2.0; see [LICENSE.txt](LICENSE.txt).
