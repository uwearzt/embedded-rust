---
marp: true
footer: © Uwe Arzt
slidenumbers: true
---

# Rust embedded

![inline, center](ewg-logo-blue-white-on-transparent-256x256.png)

*mail@uwe-arzt.de*
*uwe-arzt.de*

---

## Embedded defined

See <https://en.wikipedia.org/wiki/Embedded_system>

In our Case: A program running on a device without Monitor and Keyboard.

Often the need to operate without (power interruption sensitive) filesystem and a boot time as short
as possible. On battery operated devices power saving modes needed.

---

## Toolchain

Dependant on the concrete Microcontroler you use:

Bluepill: STM32F107RB -> thumbv7m-none-eabi
Nucleo: STM32F407 -> thumbv7em-none-eabihf

```zsh
rustup install target thumbv7em-none-eabihf
brew install cask segger-jlink
```

You also need a gnu toolchain for your target, i.e.

<https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads>

Possible targets can be listed with:

```zsh
rustup target list
```

---

## Bare Metal

**no-std** crates required

Check your dependencies

```zsh
cargo install cargo-nono

cargo nono check
as5048a: ✅
embedded-hal: ✅
linux-embedded-hal: ❌
```


---

## Blinky

```rust
```

---

## embedded-hal

<https://crates.io/crates/embedded-hal>

---

## linux-embedded-hal

---

## stm32-embedded-hal