# PolyAI

PolyAI is a AI model designed to play the game PolyTrack.

## Roadmap

- 🟡 PolyTrack simulation environment in C++
- 🔴 Optimized C++ simulation environment
- 🔴 Basic PPO model
- 🔴 Distributed training network
- 🔴 Advanced training and hyper-parameter tuning
- TBD...

## Building

Windows is not supported due to WasmTime not being available on Windows. Please use WSL.

Pre-requisites:

- [WASI SDK](https://github.com/WebAssembly/wasi-sdk)
- [Wasm Time](https://github.com/bytecodealliance/wasmtime)

1. Clone the repository with submodules:

    ```bash
    git clone --recurse-submodules https://github.com/SpideyZac/polyai.git
    cd polyai
    ```

2. Set your `WASI_SDK` environment variable to point to your WASI SDK installation:

    ```bash
    export WASI_SDK=/path/to/wasi-sdk
    ```

3. Build and run the project:

    ```bash
    make
    ```

## Formatting

This project uses `clang-format` for code formatting. To format the code, run:

```bash
./scripts/format.sh
```

## License

PolyAI itself is licensed under the MIT License. See the `LICENSE` file for details. `ammo.js` & `Bullet Physics` are licensed under their own respective licenses.
See the `ammo.js/LICENSE` and `ammo.js/bullet/LICENSE` files for details.
