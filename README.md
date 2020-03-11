<p align="center">
  CLI tool with Scala, Picoli, GraalVM and TFLite
</p>

<p align="center">
  <a href="https://github.com/mycaule/tflite-cli-example/actions"><img src="https://github.com/mycaule/tflite-cli-example/workflows/Scala%20CI/badge.svg?branch=master" alt="Build Status"></a>
  <br>
  <br>
</p>

### Pre-requisites

#### TODO

Refactor this code

https://github.com/lmoroney/dlaicourse/tree/master/TensorFlow%20Deployment/Course%202%20-%20TensorFlow%20Lite/Week%202/Examples/Android%20Apps

#### Install GraalVM

1. Download GraalVM Community Edition from https://github.com/graalvm/graalvm-ce-builds/releases.
2. Add `bin` directory to `PATH`
3. Install `native-image` command
  ```
  $ gu install native-image
  ```

#### Build

1. Build the project
  ```
  $ sbt graalvm-native-image:packageBin
  ```
2. Run the command
  ```
  $ ./target/graalvm-native-image/picocli-scala-example
  Missing required parameter: <file>
  Usage: checksum [-hV] [-a=<algorithm>] <file>
  Prints the checksum (MD5 by default) of a file to STDOUT.
        <file>      The file whose checksum to calculate.
    -a, --algorithm=<algorithm>
                    MD5, SHA-1, SHA-256, ...
    -h, --help      Show this help message and exit.
    -V, --version   Print version information and exit.
  ```


### References

- [Coursera - Device-based Models with Tensorflow Lite](https://www.coursera.org/learn/device-based-models-tensorflow), [code samples](https://github.com/lmoroney/dlaicourse/tree/master/TensorFlow%20Deployment/Course%202%20-%20TensorFlow%20Lite)
- [`takezoe/picocli-scala-example`](https://github.com/takezoe/picocli-scala-example)

