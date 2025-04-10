# Table of Contents

- [rustup](#rustup)
- [rustc](#rustc)
- [cargo](#cargo)

```
rustup 1.28.1 (f9edccde0 2025-03-05)

The Rust toolchain installer

Usage: rustup[EXE] [OPTIONS] [+toolchain] [COMMAND]

Commands:
  show         Show the active and installed toolchains or profiles
  update       Update Rust toolchains and rustup
  check        Check for updates to Rust toolchains and rustup
  default      Set the default toolchain
  toolchain    Modify or query the installed toolchains
  target       Modify a toolchain's supported targets
  component    Modify a toolchain's installed components
  override     Modify toolchain overrides for directories
  run          Run a command with an environment configured for a given toolchain
  which        Display which binary will be run for a given command
  doc          Open the documentation for the current toolchain
  man          View the man page for a given command
  self         Modify the rustup installation
  set          Alter rustup settings
  completions  Generate tab-completion scripts for your shell
  help         Print this message or the help of the given subcommand(s)

Arguments:
  [+toolchain]  Release channel (e.g. +stable) or custom toolchain to set override

Options:
  -v, --verbose  Set log level to 'DEBUG' if 'RUSTUP_LOG' is unset
  -q, --quiet    Disable progress output, set log level to 'WARN' if 'RUSTUP_LOG' is unset
  -h, --help     Print help
  -V, --version  Print version

Discussion:
    Rustup installs The Rust Programming Language from the official
    release channels, enabling you to easily switch between stable,
    beta, and nightly compilers and keep them updated. It makes
    cross-compiling simpler with binary builds of the standard library
    for common platforms.

    If you are new to Rust consider running `rustup doc --book` to
    learn Rust.
```

---

## rustc

```
Usage: rustc [OPTIONS] INPUT

Options:
    -h, --help          Display this message
        --cfg SPEC      Configure the compilation environment.
                        SPEC supports the syntax `NAME[="VALUE"]`.
        --check-cfg SPEC
                        Provide list of expected cfgs for checking
    -L [KIND=]PATH      Add a directory to the library search path. The
                        optional KIND can be one of dependency, crate, native,
                        framework, or all (the default).
    -l [KIND[:MODIFIERS]=]NAME[:RENAME]
                        Link the generated crate(s) to the specified native
                        library NAME. The optional KIND can be one of
                        static, framework, or dylib (the default).
                        Optional comma separated MODIFIERS
                        (bundle|verbatim|whole-archive|as-needed)
                        may be specified each with a prefix of either '+' to
                        enable or '-' to disable.
        --crate-type [bin|lib|rlib|dylib|cdylib|staticlib|proc-macro]
                        Comma separated list of types of crates
                        for the compiler to emit
        --crate-name NAME
                        Specify the name of the crate being built
        --edition 2015|2018|2021|2024
                        Specify which edition of the compiler to use when
                        compiling code. The default is 2015 and the latest
                        stable edition is 2024.
        --emit [asm|llvm-bc|llvm-ir|obj|metadata|link|dep-info|mir]
                        Comma separated list of types of output for the
                        compiler to emit
        --print [crate-name|file-names|sysroot|target-libdir|cfg|check-cfg|calling-conventions|target-list|target-cpus|target-features|relocation-models|code-models|tls-models|target-spec-json|all-target-specs-json|native-static-libs|stack-protector-strategies|link-args|deployment-target]
                        Compiler information to print on stdout
    -g                  Equivalent to -C debuginfo=2
    -O                  Equivalent to -C opt-level=3
    -o FILENAME         Write output to <filename>
        --out-dir DIR   Write output to compiler-chosen filename in <dir>
        --explain OPT   Provide a detailed explanation of an error message
        --test          Build a test harness
        --target TARGET Target triple for which the code is compiled
    -A, --allow LINT    Set lint allowed
    -W, --warn LINT     Set lint warnings
        --force-warn LINT
                        Set lint force-warn
    -D, --deny LINT     Set lint denied
    -F, --forbid LINT   Set lint forbidden
        --cap-lints LEVEL
                        Set the most restrictive lint level. More restrictive
                        lints are capped at this level
    -C, --codegen OPT[=VALUE]
                        Set a codegen option
    -V, --version       Print version info and exit
    -v, --verbose       Use verbose output

Additional help:
    -C help             Print codegen options
    -W help             Print 'lint' options and default settings
    --help -v           Print the full set of options rustc accepts
```

---

## cargo

```
Rust's package manager

Usage: cargo [+toolchain] [OPTIONS] [COMMAND]
       cargo [+toolchain] [OPTIONS] -Zscript <MANIFEST_RS> [ARGS]...

Options:
  -V, --version                  Print version info and exit
      --list                     List installed commands
      --explain <CODE>           Provide a detailed explanation of a rustc error message
  -v, --verbose...               Use verbose output (-vv very verbose/build.rs output)
  -q, --quiet                    Do not print cargo log messages
      --color <WHEN>             Coloring: auto, always, never
  -C <DIRECTORY>                 Change to DIRECTORY before doing anything (nightly-only)
      --locked                   Assert that `Cargo.lock` will remain unchanged
      --offline                  Run without accessing the network
      --frozen                   Equivalent to specifying both --locked and --offline
      --config <KEY=VALUE|PATH>  Override a configuration value
  -Z <FLAG>                      Unstable (nightly-only) flags to Cargo, see 'cargo -Z help' for details
  -h, --help                     Print help

Commands:
    build, b    Compile the current package
    check, c    Analyze the current package and report errors, but don't build object files
    clean       Remove the target directory
    doc, d      Build this package's and its dependencies' documentation
    new         Create a new cargo package
    init        Create a new cargo package in an existing directory
    add         Add dependencies to a manifest file
    remove      Remove dependencies from a manifest file
    run, r      Run a binary or example of the local package
    test, t     Run the tests
    bench       Run the benchmarks
    update      Update dependencies listed in Cargo.lock
    search      Search registry for crates
    publish     Package and upload this package to the registry
    install     Install a Rust binary
    uninstall   Uninstall a Rust binary
    ...         See all commands with --list

See 'cargo help <command>' for more information on a specific command.
```

---

Let me know if you want this exported to a file or tweaked for a specific platform (like GitHub README style).