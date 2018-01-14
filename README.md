# TensorFlow-Wheels

The TensorFlow wheels built by myself.

If you are using computer similar to mine, you can use these wheels.

## My computer setup

I'm using MacBook Pro 15-inch Mid 2015.

### CPU

Intel Core i7-4770HQ @ 2.20GHz

CPU features for optimization: SSE4.1, SSE4.1, AVX, AVX2, FMA

> *Note: My computer supports Intel's MKL, so linux wheels are optimzed with MKL. On the other hand, macOS wheels is not built with MKL support but I will optimize with it when TensorFlow supports MKL on macOS.*

## Linux wheels

| Version | Build command |
| ------- | ------------- |
| v1.4.1  | `bazel build --config=opt --config=mkl --copt=-mavx --copt=-mavx2 --copt=-msse4.1 --copt=-msse4.2 --copt=-mfma //tensorflow/tools/pip_package:build_pip_package` |

## macOS wheels

Coming soon!
