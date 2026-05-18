# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.47.0](https://github.com/bearcove/rediff/compare/v0.46.1...v0.47.0) - 2026-05-18

### Other

- consistent unchanged gray + stronger light contrast
- OSC-11 dark/light auto-detection + light theme
- symmetric LCH-derived dark theme (consistent deleted/inserted)
- mute unchanged tuple elements
- no spaces inside tuple parens (Failed("panic"), not Failed( "panic" ))
- confusable-string changes show a per-character codepoint breakdown
- paren-style tuples + fix missing space before brace
- per-member set diffs
- show the value when exactly one field is unchanged inline
- single-pass ordered sequence build + ValueChange node
- None renders as ∅; Option transitions are inline value changes
- compact one-line inline form for scalar-only changes
- recurse 1:1 sequence substitutions for related elements
- correct edit-distance so common elements are kept
- fix wholly deleted/inserted subtree rendering (enums)
- name collapsed unchanged fields (.. a, b unchanged)
- changed values render inline as 'name: old → new'
- Add diff gallery example; stop leaking XML @-prefix into Rust/JSON
- Render mixed/map diffs as a clean line-by-line unified diff
- Route assert macros through the layout renderer
- Make byte diff a real byte-level diff with per-byte highlighting
- Name unchanged fields in legacy diff display
- Add hex-dump diffing for byte buffers

## [0.46.1](https://github.com/bearcove/rediff/compare/v0.46.0...v0.46.1) - 2026-05-07

### Fixed

- fix clippy warnings (sort_by_key, collapsible_match)
- Option<T> was falsely equal after facet 0.46 upgrade
