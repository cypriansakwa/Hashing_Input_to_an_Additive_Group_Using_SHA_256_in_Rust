## Overview
This Rust program demonstrates how to hash an input to an additive group using the SHA-256 cryptographic hash function. The resulting hash is reduced modulo a large prime number, effectively mapping the hash to an element within the additive group defined by the prime.

## Features
- Hashes arbitrary input data using SHA-256.
- Converts the SHA-256 output into a large integer.
- Maps the hashed value to an additive group by computing the hash modulo a specified prime.

## Requirements
- Rust installed on your machine. (If Rust is not installed, follow the instructions on the [official Rust website](https://www.rust-lang.org/tools/install) to install it).
- `num-bigint` crate for handling large integers.
- `sha2` crate for the SHA-256 hashing algorithm.
- `num-traits` crate for converting between types.
- `hex` crate for encoding/decoding hexadecimal strings.

## How It Works
1. The input is hashed using SHA-256.
2. The hash result, a 256-bit value, is converted into an integer.
3. The integer is reduced modulo a prime number, which is used to define an additive group.
4. The result is an element of the additive group.

## Example
This example hashes the input string `"Hello, World!"` and maps the resulting hash to an additive group modulo the prime `340282366920938463463374607431768211507` (a large 128-bit prime).

## Input:
>```
>let input = b"Hello, World!";

### Modifying the Input
- You can change the input string by modifying the input variable. For example:
>```
>let input = b"Your new input here!";


## Contributing
  - If you intend to contribute to this project, fork the repository and make a pull request.

## Usage
- To use this code, you can clone the repository.
- Compile the Rust code using cargo:
>```
>cargo build
>cargo run
## Output
- When you run the program, the output will be an element of the group represented by an integer:
>```
>Hashed to additive group: 194190417574819553442057220677104150407

## Acknowledgments
- Rust
### Clone the repository or copy the source code into a Rust project.
```bash
   git clone https://github.com/Hashing_Input_to_an_Additive_Group_Using_SHA_256_in_Rust.git
   cd Hashing_Input_to_an_Additive_Group_Using_SHA_256_in_Rust
