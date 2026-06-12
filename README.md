## AWS C SDKUTILS

C99 library implementing AWS SDK specific utilities. Includes utilities for ARN
parsing, reading AWS profiles, etc...

## License

This library is licensed under the Apache 2.0 License.

## Usage

### Building

CMake 3.9+ is required to build.

`<install-path>` must be an absolute path in the following instructions.


#### Building aws-c-sdkutils

```
git clone git@github.com:awslabs/aws-c-common.git
cmake -S aws-c-common -B aws-c-common/build -DCMAKE_INSTALL_PREFIX=<install-path>
cmake --build aws-c-common/build --target install

git clone git@github.com:awslabs/aws-c-sdkutils.git
cmake -S aws-c-sdkutils -B aws-c-sdkutils/build -DCMAKE_INSTALL_PREFIX=<install-path> -DCMAKE_PREFIX_PATH=<install-path>
cmake --build aws-c-sdkutils/build --target install
```

<!-- PLATFORM_SUPPORT_START -->
# Platform Support

## Tier 1 — Fully Supported & Tested in CI

| Platform | Architecture |
|----------|--------------|
| Fedora-34 | x64 |
| al2 | x64 |
| macOS-14 | x64, arm64 |
| manylinux2014 | x64, x86 |
| openSUSE-leap | x64 |
| rhel8 | x64 |
| ubuntu-24.04 | x86 |
| windows 11 | x64, x86 |

## Tier 2 — Supported (Not Tested in CI)

| Platform | Architecture |
|----------|--------------|

## Supported Tools

| Name | Version | Platforms |
|------|---------|-----------|
| clang | 6+ | All |
| gcc | 4.8+ | All |
| msvc | 17 | windows |

<!-- PLATFORM_SUPPORT_END -->
