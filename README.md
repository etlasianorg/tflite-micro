<!--ts-->
   * [TensorFlow Lite for Microcontrollers](#tensorflow-lite-for-microcontrollers)
   * [Build Status](#build-status)
      * [Official Builds](#official-builds)
      * [Community Supported TFLM Examples](#community-supported-tflm-examples)
      * [Community Supported Kernels and Unit Tests](#community-supported-kernels-and-unit-tests)
   * [Contributing](#contributing)
   * [Getting Help](#getting-help)
   * [Additional Documentation](#additional-documentation)
   * [RFCs](#rfcs)

<!-- Added by: advaitjain, at: Mon 04 Oct 2021 11:23:57 AM PDT -->

<!--te-->

# TensorFlow Lite for Microcontrollers

TensorFlow Lite for Microcontrollers is a port of TensorFlow Lite designed to
run machine learning models on DSPs, microcontrollers and other devices with
limited memory.

Additional Links:
 * [Tensorflow github repository](https://github.com/tensorflow/tensorflow/)
 * [TFLM at tensorflow.org](https://www.tensorflow.org/lite/microcontrollers)

# Build Status

 * [GitHub Status](https://www.githubstatus.com/)

## Official Build

Build Type       |    Status     |
-----------      | --------------|
CI (Linux)       | [![CI](https://github.com/tensorflow/tflite-micro/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/tensorflow/tflite-micro/actions/workflows/ci.yml?query=event%3Aschedule) |
Code Sync        | [![Sync from Upstream TF](https://github.com/tensorflow/tflite-micro/actions/workflows/sync.yml/badge.svg)](https://github.com/tensorflow/tflite-micro/actions/workflows/sync.yml) |


## Community Supported TFLM Examples
This table captures platforms that TFLM has been ported to. Please see
[New Platform Support](tensorflow/lite/micro/docs/new_platform_support.md) for
additional documentation.

Platform      |    Status     |
-----------     | --------------|
Arduino         | [![Arduino](https://github.com/tensorflow/tflite-micro-arduino-examples/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/tensorflow/tflite-micro-arduino-examples/actions/workflows/ci.yml) [![Antmicro](https://github.com/antmicro/tensorflow-arduino-examples/actions/workflows/test_examples.yml/badge.svg)](https://github.com/antmicro/tensorflow-arduino-examples/actions/workflows/test_examples.yml) |
ESP32           | [![ESP32](https://github.com/espressif/tflite-micro-esp-examples/actions/workflows/build.yml/badge.svg)](https://github.com/espressif/tflite-micro-esp-examples/actions/workflows/build.yml) |
Sparkfun Edge   | [![Sparkfun Edge](https://github.com/advaitjain/tflite-micro-sparkfun-edge-examples/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/advaitjain/tflite-micro-sparkfun-edge-examples/actions/workflows/ci.yml)


## Community Supported Kernels and Unit Tests
This is a list of targets that have optimized kernel implementations and/or run
the TFLM unit tests using software emulation or instruction set simulators.

Build Type      |    Status     |
-----------     | --------------|
Cortex-M        | [![Cortex-M](https://github.com/tensorflow/tflite-micro/actions/workflows/cortex_m.yml/badge.svg)](https://github.com/tensorflow/tflite-micro/actions/workflows/cortex_m.yml) |
Hexagon         | [![Hexagon](https://github.com/tensorflow/tflite-micro/actions/workflows/hexagon.yml/badge.svg?event=schedule)](https://github.com/tensorflow/tflite-micro/actions/workflows/hexagon.yml) |
RISC-V          | [![RISC-V](https://github.com/tensorflow/tflite-micro/actions/workflows/riscv.yml/badge.svg)](https://github.com/tensorflow/tflite-micro/actions/workflows/riscv.yml) |
Xtensa          | [![Xtensa](https://github.com/tensorflow/tflite-micro/actions/workflows/xtensa.yml/badge.svg?event=schedule)](https://github.com/tensorflow/tflite-micro/actions/workflows/xtensa.yml?query=event%3Aschedule) [![Xtensa](https://raw.githubusercontent.com/advaitjain/tflite-micro/local-continuous-builds/tensorflow/lite/micro/docs/local_continuous_builds/xtensa-build-status.svg)](https://github.com/advaitjain/tflite-micro/tree/local-continuous-builds/tensorflow/lite/micro/docs/local_continuous_builds/xtensa.md#summary) |


# Contributing
See our [contribution documentation](CONTRIBUTING.md).

# Getting Help

A [Github issue](https://github.com/tensorflow/tflite-micro/issues/new/choose)
should be the primary method of getting in touch with the TensorFlow Lite Micro
(TFLM) team.

The following resources may also be useful:

1.  SIG Micro [email group](https://groups.google.com/a/tensorflow.org/g/micro)
    and
    [monthly meetings](http://doc/1YHq9rmhrOUdcZnrEnVCWvd87s2wQbq4z17HbeRl-DBc).

1.  SIG Micro [gitter chat room](https://gitter.im/tensorflow/sig-micro).

1. For questions that are not specific to inference with TFLM (for example
   model conversion and quantization) please use the following resources:
   * Send an email to the [TfLite Mailing List](https://groups.google.com/a/tensorflow.org/g/tflite)
   * Create a [TensorFlow Lite Converter Issue](https://github.com/tensorflow/tensorflow/issues/new?assignees=&labels=TFLiteConverter&template=60-tflite-converter-issue.md)
   * Create an issue in the [model optimization toolkit](https://github.com/tensorflow/model-optimization) GitHub repository
   * Create an issue in the [model optimization toolkit](https://github.com/tensorflow/model-optimization) GitHub repository


# Additional Documentation

 * [Continuous Integration](docs/continuous_integration.md)
 * [Benchmarks](tensorflow/lite/micro/benchmarks/README.md)
 * [Profiling](tensorflow/lite/micro/docs/profiling.md)
 * [Memory Management](tensorflow/lite/micro/docs/memory_management.md)
 * [Porting Reference Kernels from TfLite to TFLM](tensorflow/lite/micro/docs/porting_reference_ops.md)
 * [Optimized Kernel Implementations](tensorflow/lite/micro/docs/optimized_kernel_implementations.md)
 * [New Platform Support](tensorflow/lite/micro/docs/new_platform_support.md)
 * [Software Emulation with Renode](tensorflow/lite/micro/docs/renode.md)
 * [Python Dev Guide](docs/python.md)
 * [Automatically Generated Files](docs/automatically_generated_files.md)

# RFCs

1. [Pre-allocated tensors](tensorflow/lite/micro/docs/rfc/001_preallocated_tensors.md)
1. [TensorFlow Lite for Microcontrollers Port of 16x8 Quantized Operators](tensorflow/lite/micro/docs/rfc/002_16x8_quantization_port.md)
