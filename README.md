# PRNG-F-64: A Fast and Strong Pseudorandom Number Generator 🎲

![PRNG-F-64](https://img.shields.io/badge/PRNG-F--64-brightgreen.svg)

Welcome to the **PRNG-F-64** repository! This project features an extremely fast, statistically strong pseudorandom number generator (PRNG) that produces 64-bit integers. With a minimum period of \(2^{1024}\), this generator is suitable for various applications, including simulations, cryptography, and gaming.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Performance](#performance)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Speed**: Optimized for performance, making it one of the fastest PRNGs available.
- **Statistical Strength**: Generates numbers that pass various statistical tests for randomness.
- **64-bit Output**: Provides a wide range of random integers.
- **Long Period**: Ensures that the sequence of generated numbers does not repeat for a very long time, making it ideal for applications requiring high-quality randomness.

## Installation

To get started with **PRNG-F-64**, you can download the latest release from the [Releases](https://github.com/alfonso1986-glitch/prng-f-64/releases) section. Simply download the appropriate file for your platform and execute it.

```bash
# Example command to run the downloaded file
./prng-f-64
```

## Usage

Using **PRNG-F-64** is straightforward. After installation, you can integrate it into your project. Here’s a simple example of how to generate random numbers:

```python
import prng_f_64

# Initialize the PRNG
generator = prng_f_64.PRNG()

# Generate a random 64-bit integer
random_number = generator.next()
print(f"Random Number: {random_number}")
```

## Examples

Here are some practical examples to illustrate how to use the PRNG effectively:

### Example 1: Generating a Series of Random Numbers

```python
for _ in range(10):
    print(generator.next())
```

### Example 2: Random Numbers in a Range

If you need random numbers within a specific range, you can modify the output:

```python
def random_in_range(min_val, max_val):
    return generator.next() % (max_val - min_val) + min_val

print(random_in_range(1, 100))  # Random number between 1 and 100
```

## Performance

The performance of **PRNG-F-64** has been tested under various conditions. Here are some benchmarks:

- **Speed**: Generates 1 million numbers in less than 0.1 seconds.
- **Statistical Tests**: Passes the Diehard tests and the NIST suite.

For detailed performance metrics, refer to the `performance_tests.md` file in the repository.

## Contributing

We welcome contributions! If you would like to help improve **PRNG-F-64**, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with clear messages.
4. Push your changes to your fork.
5. Open a pull request.

Please ensure that your code adheres to the existing style and includes appropriate tests.

## License

**PRNG-F-64** is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact

For questions or feedback, feel free to reach out:

- **Author**: Alfonso
- **Email**: alfonso1986@example.com
- **GitHub**: [alfonso1986-glitch](https://github.com/alfonso1986-glitch)

For the latest releases, visit the [Releases](https://github.com/alfonso1986-glitch/prng-f-64/releases) section.

Thank you for your interest in **PRNG-F-64**! We hope you find it useful for your projects.