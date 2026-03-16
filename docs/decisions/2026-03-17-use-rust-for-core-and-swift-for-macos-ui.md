# Use Rust for the core and Swift for the macOS UI

## Context and Problem Statement

Nagi should be performant and also feel nice to use on macOS.

The main question was which systems language to use for the application foundation, considering Rust, Go, Zig, and C++.

## Considered Options

- Rust
  - Alacritty, WezTerm, and Warp known to use Rust. Probably for performance.
- Go
  - kitty uses Go along with Python and C
- Zig
  - Ghostty's core known to use Zig.
- C++
  - Windows Terminal uses C++.

## Decision Outcome

Chosen option: "Rust", because it is a strong fit for a performance-sensitive terminal core while keeping implementation risk lower than C++ and ecosystem risk lower than Zig.

For the macOS application layer, use Swift with Apple's native UI frameworks so the app can feel at home on Mac instead of forcing the entire product through one cross-platform stack.
