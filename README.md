# RustCoder Projects

A collection of utility tools built with Rust, featuring both CLI and TUI (Terminal User Interface) applications.

## Projects Overview

### 1. File Encrypter (`file-encrypter`)
A secure file and directory encryption utility.
- **Encryption:** Uses AES-256-GCM for authenticated encryption.
- **Key Derivation:** Employs Argon2id password hashing for robust security.
- **Features:** 
  - Single file and recursive directory encryption.
  - Progress bar integration using `indicatif`.
  - Secure password-based key derivation with random salting.

### 2. HTTP API Client (`http-api-client`)
A user-friendly CLI tool for making HTTP requests, inspired by `curl` and `httpie`.
- **Features:**
  - Support for common HTTP methods (GET, POST, PUT, DELETE, etc.).
  - Pretty-printed and colorized JSON output.
  - Request profiles for saving and reusing common endpoints.
  - Header management and body support.
- **Implementation:** Built using `reqwest` for networking and `serde_json` for processing.

### 3. Markdown Previewer (`markdown-previewer`)
A terminal-based Markdown renderer with a focus on readability.
- **Features:**
  - Renders headings, paragraphs, lists, blockquotes, and code blocks.
  - Scrollable view with keyboard navigation (Up/Down, PgUp/PgDn).
  - TUI interface built with `ratatui` and `crossterm`.
- **Usage:** Run with a path to a markdown file to preview it directly in your terminal.

### 4. Pomodoro Timer (`pomodoro-timer`)
A productivity-focused TUI application for managing work and break intervals.
- **Features:**
  - Customizable work and break durations.
  - Desktop notifications via `notify-rust` when sessions start or end.
  - Real-time session statistics (total work/break time, sessions completed).
  - Clean TUI interface built with `ratatui`.

---

## Getting Started

Each project is a standalone Rust crate. To build and run any of them, ensure you have [Rust and Cargo](https://rustup.rs/) installed, then navigate to the project directory and use `cargo run`.

### Example: Running the Pomodoro Timer
```bash
cd pomodoro-timer
cargo run
```

### Example: Encrypting a file
```bash
cd file-encrypter
cargo run -- encrypt-file --password "your-password" input.txt output.enc
```

## License
Refer to individual folders for license information if available.
