# Changelog

## Unreleased

* Increase MSRV to 1.59.0 because of `rayon-core v1.11.0`.

## 0.14.1 (2022-07-14)

* Undo performance regression from removing `hashbrown` by using `ahash` hasher

## 0.14.0 (2022-07-12)

* Removed dependency `hashbrown` since it is part of `std` since Rust 1.36
* Removed dependency `mopa` since it is unmaintained and has a potential vulnerability

## 0.13.0 (2022-06-22)

* Bumped dependency of `hashbrown` to `0.12`
* Bumped dependency of `arrayvec` to `0.7.2`.
* Add getters to DispatcherBuilder
* increase minimal rust version to `1.56.1`
* improve performance by switching to `compare_exchange_weak`

## 0.12.0 (2021-03-21)

* Bumped dependency of `hashbrown` to `0.11`

## 0.11.1 (2021-03-10)

* Bumped dependency of smallvec as there was an open RUSTSEC issue

## 0.11.0 (2020-12-21)

* Batch dispatching ergonomics -- remove `unsafe` on the user side. ([#197], [#198]).
* Bumped dependency versions. ([#203], [#204])

[#197]: https://github.com/amethyst/shred/issues/197
[#198]: https://github.com/amethyst/shred/pull/198
[#203]: https://github.com/amethyst/shred/issues/203
[#204]: https://github.com/amethyst/shred/pull/204

## 0.10.2 (2020-02-13)

### Changed

* Bumped dependency versions. ([#193])

[#193]: https://github.com/amethyst/shred/pull/193

## 0.10.1 (2020-02-12)

### Changed

* Bump `tynm` to `0.1.3`. ([#187])
* Implement `Resource` for `!Send + !Sync` types when `"parallel"` feature is disabled. ([#186])

[#186]: https://github.com/amethyst/shred/pull/186
[#187]: https://github.com/amethyst/shred/pull/187

## 0.10.0 (2019-12-31)

### Changed

* Updated `arrayvec` from `0.4` to `0.5`. ([#176])
* Updated `rayon` from `1.1` to `1.3`. ([#180])
* Updated `smallvec` from `0.6` to `1.1`. ([#180])
* `shred-derive`: Updated `syn`, `quote`, `proc-macro2` to `1.0`. ([#176])
* ***Minimum Supported Rust Version updated to `1.38.0`***. ([#176])
* Improved clarity of fetch panic message. ([#182])

[#176]: https://github.com/amethyst/shred/issues/176
[#180]: https://github.com/amethyst/shred/issues/180
[#182]: https://github.com/amethyst/shred/issues/182

## 0.9.4 (2019-11-16)

### Added

* Batch dispatching. ([#147])

[#147]: https://github.com/amethyst/shred/pull/147
