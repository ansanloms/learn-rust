# Rust のインストール

## Windows

winget で Rustup を入れる。別途 Visual Studio Build Tools 2019 が必要。

```bash
winget install Rustlang.Rustup
winget install Microsoft.VisualStudio.2019.BuildTools
```

Visual Studio Installer を開いて、「インストール済み」タブ上にある「Visual Studio Build Tools 2019」の「変更(M)」を押下。「個別のコンポーネント」タブを選択し、以下を選択してインストールする。

- Windows 10 SDK
- MSVC v140 - VS 2015 C++ ビルド ツール (v14.00)

Rustup から Rust をインストールする。

```bash
rustup update
rustc --version
```

## rustfmt

```bash
rustup component add rustfmt
```
