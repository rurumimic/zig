# zig

- [zig](https://ziglang.org/)
  - [github](https://github.com/ziglang): [zig](https://github.com/ziglang/zig)
  - [tools](https://ziglang.org/learn/tools)
  - [releases](https://ziglang.org/download)
    - [install](https://github.com/ziglang/zig/wiki/Install-Zig-from-a-Package-Manager)
  - [news](https://ziglang.org/news)
- [doc](https://ziglang.org/documentation/master/)
  - [learn](https://ziglearn.org/)
  - [ziglings](https://github.com/ratfactor/ziglings)
- [community](https://github.com/ziglang/zig/wiki/Community)
- editors
  - [zls](https://github.com/zigtools/zls): [install](https://install.zigtools.org/)
  - [zig.vim](https://github.com/ziglang/zig.vim)

---

## Start

### Install

```bash
curl -O https://ziglang.org/builds/zig-linux-x86_64-X.Y.Z.tar.xz
tar xf zig-linux-x86_64-X.Y.Z.tar.xz
mv zig-linux-x86_64-X.Y.Z ~/.zig
```

```bash
# ~/.zshrc
export PATH="$PATH:$HOME/.zig"
```

```bash
zig version
```

### Hello World

[src/helloworld/src/main.zig](src/helloworld/src/main.zig)

```bash
# helloworld/
zig init-exe
```

```bash
helloworld/
├── build.zig
└── src/
    └── main.zig
```

```bash
zig build run

Hello, world!
```

### zls

- zigtools/[zls](https://github.com/zigtools/zls)

```bash
git clone https://github.com/zigtools/zls
cd zls
zig build -Doptimize=ReleaseSafe -Ddata_version=X.Y.Z
```

### Editor

#### VSCode

- extension
  - [zig](https://marketplace.visualstudio.com/items?itemName=tiehuis.zig)
  - [zls](https://marketplace.visualstudio.com/items?itemName=AugusteRame.zls-vscode)

#### SpaceVim

- spacevim layer
  - [zig](https://spacevim.org/layers/lang/zig/)
- [zig.vim](https://github.com/ziglang/zig.vim)

Open SpaceVim Configuration File: `SPC f v d`

```toml
[options]
  autocomplete_method = "coc"

[[layers]]
  name = "autocomplete"

[[layers]]
  name = "lang#zig"
```

in SpaceVim:

```bash
:CocInstall coc-zls
```

---

## Code

### Learn

1. [Basics](src/learn/basics/README.md)
1. [Standard Pattenrs](src/learn/standard_patterns/README.md)
1. [Build System](src/learn/build_system/README.md)
1. [Working with C](src/learn/working_with_c/README.md)
1. [Async](src/learn/async/README.md)

