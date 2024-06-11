# 0x02. Python - Async Comprehension

This repository contains tasks related to asynchronous programming in Python, focusing on async generators, async comprehensions, and measuring runtime for asynchronous tasks.

## Learning Objectives

By the end of this project, you should be able to:

- Write an asynchronous generator
- Use async comprehensions
- Type-annotate generators

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using `python3` (version 3.7)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/env python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the `pycodestyle` style (version 2.5.x)
- The length of your files will be tested using `wc`
- All your modules should have a documentation (use `python3 -c 'print(__import__("my_module").__doc__)'`)
- All your functions should have a documentation (use `python3 -c 'print(__import__("my_module").my_function.__doc__)'`)
- A documentation is not a simple word; it’s a real sentence explaining the purpose of the module, class, or method (the length of it will be verified)
- All your functions and coroutines must be type-annotated

## Tasks

### Task 0: Async Generator

- **File**: `0-async_generator.py`
- **Description**: Write a coroutine called `async_generator` that takes no arguments. The coroutine will loop 10 times, each time asynchronously wait 1 second, then yield a random number between 0 and 10. Use the `random` module.

### Task 1: Async Comprehensions

- **File**: `1-async_comprehension.py`
- **Description**: Import `async_generator` from the previous task and write a coroutine called `async_comprehension` that takes no arguments. The coroutine will collect 10 random numbers using an async comprehending over `async_generator`, then return the 10 random numbers.

### Task 2: Run Time for Four Parallel Comprehensions

- **File**: `2-measure_runtime.py`
- **Description**: Import `async_comprehension` from the previous file and write a `measure_runtime` coroutine that will execute `async_comprehension` four times in parallel using `asyncio.gather`. `measure_runtime` should measure the total runtime and return it. Notice that the total runtime is roughly 10 seconds.

## Explanation

The total runtime is approximately 10 seconds because each `async_comprehension` coroutine runs for about 10 seconds (as it waits 1 second for each of 10 iterations). Running four of these coroutines in parallel using `asyncio.gather` means that they all start and run simultaneously, so the overall runtime is the time taken by one coroutine, which is about 10 seconds.

## Author

Carrie

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
