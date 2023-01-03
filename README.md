Swag to OpenAPI Converter
---
Built with ❤️

This package was created because https://github.com/swaggo/swag does not support openapi 3.0.

It is essentially a copy of swag's main.go and added kin-openapi conversion functions.

## Installation
```bash
go install github.com/dimasdanz/swag-openapi3
```
## How To
As it's just a copy, all the flag in [swag's cli](https://github.com/swaggo/swag#swag-cli) should work.
One caveat, the outputType is hardcoded to json file because kin-openapi's converter does not work well with other type.

Run swag's comment format. Assuming GOPATH BIN is in the env's PATH
```bash
openapi fmt
```
Generate OpenAPI 3.0
```bash
openapi init --output out -requiredByDefault
```
