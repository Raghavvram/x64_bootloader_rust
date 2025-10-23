# x64 Bootloader

A simple bootloader for x86_64 systems written in Rust.

## Usage

### Prerequisites

- [rustup](https://rustup.rs/)
- [QEMU](https://www.qemu.org/)

### Building and Running

1. **Set the default Rust toolchain to nightly:**
   ```sh
   rustup default nightly
   ```

2. **Add the `llvm-tools-preview` component:**
   ```sh
   rustup component add llvm-tools-preview
   ```

3. **Build the bootloader:**
   ```sh
   cargo build
   ```

4. **Run the bootloader in QEMU:**
   ```sh
   qemu-system-x86_64 -drive format=raw,file=target/x86_64-bootloader/debug/x64_bootloader
   ```
