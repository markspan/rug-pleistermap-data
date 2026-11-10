# RUG bandaid dispensers: dataset

`dispensers.geojson` holds the bandaid dispensers in University of Groningen buildings.

- Read by the public [Bandaid Finder](https://github.com/markspan/rug-pleistermap).
- Written by the Bandaid Editor: every save is one commit here, so the history is the
  full log of additions, moves and fill-level checks. Undo a bad change with `git revert`.

Each feature is a point (EPSG:4326) with properties `floor` (RUG Maps floor code such as
`00`, `0T`, `-S`), `building`, `room`, `note`, `fill` (0 to 100, or null if never checked)
and `checkedAt` (ISO time of the last check).

This repository holds data only, so the Editor's token (scoped to this repository) can
never change app code.
