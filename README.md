# xrpl-hooks-prototyping

This project is an exploration of [XRPL Hooks](https://xrpl-hooks.readme.io/).

## Links

### Hooks Docs
* [https://hooks.xrpl.org](https://hooks.xrpl.org/)
  * [Hooks Builder](https://hooks-builder.xrpl.org/develop)
* [Compiling Hoooks](https://xrpl-hooks.readme.io/docs/compiling-hooks)
* [Compiling C to WASM](https://developer.mozilla.org/en-US/docs/WebAssembly/C_to_wasm)
* [Hooks Cleaner](https://github.com/XRPLF/hook-cleaner-c)
* WASMER
  * [https://wasmer.io/](https://wasmer.io/)
  * [wasienv](https://github.com/wasienv/wasienv)
* [Vegas Hook Example](https://www.youtube.com/watch?v=dK6n_tChTFM)

### Hooks Testnet
* [Faucet](https://hooks-testnet-v3.xrpl-labs.com/)

## Test Account

Address: `rNhn5hQcmxPFq7V7jMncc5WVoeWLwrPWA9`
Secret: `ss38hjx9H7UH5dNpZSaBDcmjPZhrN`

## Setup Dev Environment

See Emscripten & WebAssembly [here](https://gist.github.com/WesThorburn/00c47b267a0e8c8431e06b14997778e4)

1. Enter the cloned directory: `cd emsdk`
2. Checkout main: `git checkout main`
3. Install the lastest sdk tools: `./emsdk install latest` 
4. Activate the latest sdk tools: `./emsdk activate latest` 
5. Activate path variables: `source ./emsdk_env.sh`
   

## Build Hook

# Test Hook (Hooks Testnet v3)
1. Build: 

  ```bash
  ./build.sh
  ```
2.Set Hook:

```bash
nodejs set_hook ss38hjx9H7UH5dNpZSaBDcmjPZhrN library
```

3. Check:

```bash
nodejs pay ss38hjx9H7UH5dNpZSaBDcmjPZhrN 1000 rNhn5hQcmxPFq7V7jMncc5WVoeWLwrPWA9
```

## TODOs
- [ ] Use WASI with a MAKEFILE (instead of emscripten)
- 