# agentum-runtime
SHA-pinned runtime binaries bundled with the Agentum desktop app

## How the binaries are made

| Release | Asset | Made by |
|---|---|---|
| `whisper-cli-v1.8.2` | `whisper-cli-darwin-arm64` | whisper.cpp v1.8.2 (Metal), built on a Mac |
| `whisper-cli-v1.8.2` | `whisper-cli-win32-x64.exe` | `.github/workflows/whisper-cli-windows.yml`: whisper.cpp v1.8.2, one self-contained .exe (Visual C++ runtime linked in, OpenMP off), so it starts on a clean Windows install |
| `kokoro-multi-lang-v1_0` | voice pack | byte-identical mirror of the upstream sherpa-onnx asset |

An asset is never replaced once published: the desktop app pins each one by sha256.
