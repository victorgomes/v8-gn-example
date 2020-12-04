# V8 embedder example built with GN

## Instructions

### Checking out source

[Get depot_tools](https://commondatastorage.googleapis.com/chrome-infra-docs/flat/depot_tools/docs/html/depot_tools_tutorial.html#_setting_up) first.

```bash
mkdir new-project
cd new-project
git clone https://github.com/victorgomes/v8-gn-example.git
gclient config https://github.com/victorgomes/v8-gn-example.git --unmanaged
cd v8-gn-example
gclient sync
```

### Build and run example

```bash
gn gen out/release
autoninja -C out/release hello-world
./out/release/hello-world
```

