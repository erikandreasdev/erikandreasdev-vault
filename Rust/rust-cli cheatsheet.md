# 🦀 Rust Core CLI Commands

A quick reference for essential Rust command-line tools and usage.

---

## 📑 Table of Contents
- [Rust Core CLI Commands](#-rust-core-cli-commands)
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

## 🔧 CLI Tools

These tools come with a standard Rust installation:

- `rustc` – The Rust compiler
- `cargo` – Package manager and build system
- `rustup` – Toolchain/version manager
- `rustdoc` – Documentation generator
- `rustfmt` – Code formatter
- `clippy` – Linter for code quality

---

## 📌 Check Rust version
```bash
rustc --version
```
Displays the installed Rust compiler version.

---

## 🔄 Update Rust
```bash
rustup update
```
Updates Rust and all installed components.

---

## ❌ Uninstall Rust
```bash
rustup self uninstall
```
Completely removes Rust from your system.

---

## ⚙️ Compile a Rust file
```bash
rustc main.rs
```
Compiles `main.rs` into an executable.

---

## ▶️ Execute the compiled file
```bash
./main
```
Runs the compiled binary.

---

## 📁 Create a new project with Cargo
```bash
cargo new project_name
```
Generates a new project structure with:
- `Cargo.toml`
- `src/main.rs`

---

## 🏗️ Build a project
```bash
cargo build
```
Compiles the project and outputs a binary in the `target/` directory.

---

## 🚀 Run a project
```bash
cargo run
```
Builds and immediately runs the project.

---

## 🔍 Check a project (analyze without building)
```bash
cargo check
```
Performs analysis for errors without building the binary (fast feedback during dev).

---

## 📄 Example `Cargo.toml`
```toml
[package]
name = "project_name"
version = "0.1.0"
edition = "2021"

[dependencies]
```

### 🔍 Explanation
- `[package]`: Project metadata
  - `name`: Project name
  - `version`: Current version
  - `edition`: Rust edition (e.g., 2021)
- `[dependencies]`: External libraries used in the project

📚 Learn more about the TOML format: [TOML Documentation](https://toml.io/en/)
