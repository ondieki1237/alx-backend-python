# Python Async IO Project

## Description
This project focuses on the use of Python’s asynchronous programming capabilities, specifically using `asyncio`. The goal is to learn how to write concurrent code using async/await syntax, execute asynchronous programs, manage tasks, and work with the `random` module to simulate real-world asynchronous tasks.

## Learning Objectives
By the end of this project, you will be able to:
- Understand and explain the `async` and `await` syntax.
- Execute asynchronous programs using `asyncio`.
- Run concurrent coroutines in an efficient manner.
- Create and manage `asyncio` tasks.
- Use the `random` module, especially the `random.uniform()` function, to generate random numbers.

## Resources
For further reading, please refer to the following resources:
- [Async IO in Python: A Complete Walkthrough](https://realpython.com/async-io-python/)
- [asyncio - Asynchronous I/O](https://docs.python.org/3/library/asyncio.html)
- [random.uniform](https://docs.python.org/3/library/random.html#random.uniform)

## Requirements
### General
- A `README.md` file, located at the root of the project folder, is mandatory.
- Allowed editors: `vi`, `vim`, `emacs`.
- All files will be interpreted/compiled on Ubuntu 18.04 LTS using `python3` (version 3.7).
- All files must end with a new line.
- All files must be executable.
- The length of the files will be tested using `wc`.
- The first line of all Python files should be exactly `#!/usr/bin/env python3`.
- Code should adhere to the `pycodestyle` style (version 2.5.x).
- All functions and coroutines must be type-annotated.
- Modules should have a proper documentation string (`__doc__`).
- Functions should have a meaningful documentation explaining their purpose.

## Project Structure

### Example: Asynchronous Function
Here is an example of how to use `async` and `await` to define an asynchronous function in Python:

```python
#!/usr/bin/env python3
"""
Module to demonstrate asynchronous programming with asyncio and random.
"""

import asyncio
import random

async def async_task():
    """
    Simulates an asynchronous task that takes a random amount of time to complete.
    """
    delay = random.uniform(1, 5)
    await asyncio.sleep(delay)
    return f"Task completed after {delay:.2f} seconds."
