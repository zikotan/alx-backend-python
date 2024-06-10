# 0x01. Python - Async Function

This repository contains tasks related to asynchronous programming in Python. The goal of these tasks is to help you understand and practice writing asynchronous functions using `async` and `await`.

## Description

The tasks in this project cover various aspects of Python's asynchronous programming, including basic syntax, concurrent coroutines, measuring execution time, and working with asynchronous tasks.

## Tasks

### Task 0: Basic Async Syntax
- **File**: `0-basic_async_syntax.py`
- **Description**: Write an asynchronous coroutine called `wait_random` that takes an integer `max_delay` (default 10) and returns a random float between 0 and `max_delay` after waiting for that float delay.

### Task 1: Concurrent Coroutines
- **File**: `1-concurrent_coroutines.py`
- **Description**: Write an asynchronous coroutine called `wait_n` that takes two integers `n` and `max_delay`. It spawns `wait_random` `n` times with the specified `max_delay` and returns the list of all delays in ascending order.

### Task 2: Measure Runtime
- **File**: `2-measure_runtime.py`
- **Description**: Write a function `measure_time` that measures the total runtime of `wait_n` and returns it divided by `n`.

### Task 3: Tasks
- **File**: `3-tasks.py`
- **Description**: Write a function `task_wait_random` that takes an integer `max_delay` and returns a `asyncio.Task` that waits for `wait_random`.

### Task 4: More Tasks
- **File**: `4-tasks.py`
- **Description**: Write a function `task_wait_n` that takes two integers `n` and `max_delay`. It spawns `task_wait_random` `n` times with the specified `max_delay` and returns the list of all delays in ascending order.

## Getting Started

To get started with this project, simply clone the repository and start exploring the Python files in each task. Each file contains a specific function or set of functions designed to help you practice and understand asynchronous programming in Python.

### Prerequisites

- Python 3.7+

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/0x01-python_async_function.git
