## 🦀 Beginner Rust Command Cheat Sheet

---

### 📦 Cargo Commands

| Command | Use | Example | Note |
|--------|-----|---------|------|
| `cargo new` | Create a new project | `cargo new my_app` | Sets up folder with `Cargo.toml` and `src/main.rs` |
| `cargo init` | Init Cargo in existing folder | `cargo init .` | Adds `Cargo.toml` and source structure |
| `cargo build` | Compile the project | `cargo build` | Use `--release` for optimized build |
| `cargo run` | Build and run | `cargo run` | Add args with `--`, e.g. `cargo run -- arg1` |
| `cargo check` | Check for errors | `cargo check` | Faster than build; no binary created |
| `cargo test` | Run tests | `cargo test` | Auto-runs all tests with `#[test]` |
| `cargo fmt` | Format code | `cargo fmt` | Requires `rustup component add rustfmt` |
| `cargo clippy` | Lint code | `cargo clippy` | Requires `rustup component add clippy` |
| `cargo doc --open` | View project docs | `cargo doc --open` | Uses comments like `///` |
| `cargo clean` | Remove build artifacts | `cargo clean` | Clears the `target/` directory |
| `cargo update` | Update dependencies | `cargo update` | Updates in `Cargo.lock` only |
| `cargo add` | Add a crate dependency | `cargo add serde` | Requires `cargo install cargo-edit` |

---

### 🦀 rustc Command

| Command | Use | Example | Note |
|--------|-----|---------|------|
| `rustc` | Compile a single file | `rustc main.rs` | No dependency management; not for projects |

---

### 🛠️ rustup Commands

| Command | Use | Example | Note |
|--------|-----|---------|------|
| `rustup update` | Update Rust toolchain | `rustup update` | Gets latest stable Rust |
| `rustup show` | Show current toolchain | `rustup show` | Helpful for debugging |
| `rustup component add` | Add tools like `clippy` or `rustfmt` | `rustup component add clippy` | Enables extra features |

---
