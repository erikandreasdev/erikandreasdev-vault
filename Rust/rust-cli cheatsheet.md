# Rust Core CLI Commands

## Table of Contents
- [Rust Core CLI Commands](#rust-core-cli-commands)
- [Check Rust version](#check-rust-version)
- [Update Rust](#update-rust)
- [Uninstall Rust](#uninstall-rust)
- [Compile a Rust file](#compile-a-rust-file)
- [Execute the compiled file](#execute-the-compiled-file)
- [Create a new project with Cargo](#create-a-new-project-with-cargo)
- [Build a project](#build-a-project)
- [Run a project](#run-a-project)
- [Check a project (analyze without building)](#check-a-project-analyze-without-building)
- [Example `Cargo.toml`](#example-cargotoml)

---

Core command-line tools that come with a Rust installation.

- `rustc` – The Rust compiler, used to compile Rust source files.
- `cargo` – The official Rust package manager and build system.
- `rustup` – Manages Rust versions and associated tools.
- `rustdoc` – Generates documentation from Rust code.
- `rustfmt` – Automatically formats Rust code.
- `clippy` – Provides lints to catch common mistakes and improve code quality.

---

### Check Rust version
```bash
rustc --version
```
Shows the currently installed Rust compiler version.

### Update Rust
```bash
rustup update
```
Updates Rust and all installed components to the latest stable versions.

### Uninstall Rust
```bash
rustup self uninstall
```
Removes Rust and all associated tools from your system.

---

### Compile a Rust file
```bash
rustc main.rs
```
Compiles a single Rust source file (`main.rs`) into a binary.

### Execute the compiled file
```bash
./main
```
Runs the compiled binary output by `rustc`.

---

### Create a new project with Cargo
```bash
cargo new project_name
```
Creates a new Rust project directory with the necessary files, including `Cargo.toml` and `src/main.rs`.

---

### Build a project
```bash
cargo build
```
Compiles the entire Cargo project and outputs a binary in the `target` directory.

### Run a project
```bash
cargo run
```
Builds and immediately runs the Rust project.

### Check a project (analyze without building)
```bash
cargo check
```
Quickly analyzes the project for errors without producing a binary—useful for fast feedback during development.

---

### Example `Cargo.toml`
```toml
[package]
name = "project_name"
version = "0.1.0"
edition = "2021"

[dependencies]
```

#### Explanation
- `[package]`: Contains metadata about the project.
  - `name`: The name of the package.
  - `version`: The current version.
  - `edition`: Specifies the Rust edition (like a language version).
- `[dependencies]`: Where you list external crates (libraries) your project uses.

For more about the TOML format, see the [official TOML documentation](https://toml.io/en/).
