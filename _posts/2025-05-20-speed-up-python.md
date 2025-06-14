---
layout: post
title: "7 Ways to Speed Up Your Python Code"
author: rayean
categories: [Tech, Programming]
image: https://rayean-mahmud.github.io/assets/images/python.jpg
---

🚀 Writing efficient Python code is essential for developers working on performance-sensitive tasks like data processing, web applications, or machine learning. In this post, you'll explore **7 proven techniques** to boost Python performance — with examples, explanations, and quick wins you can implement right away.

---

## ✅ 1. Profile Your Code Before Optimizing

Before making changes, **identify the real bottlenecks** using profiling tools:

```python
import cProfile

def main():
    # Your code
    ...

cProfile.run('main()')
```

🔍 Use tools like `timeit`, `line_profiler`, or `snakeviz` to dig deeper.

> ⚠️ Don't optimize blindly. Focus only on the actual slow spots.

---

## ⚡ 2. Use Built-In Functions and Libraries

Python’s built-ins (written in C) are **much faster** than custom logic:

```python
# Slower version
s = 0
for i in range(1000000):
    s += i

# Faster version
s = sum(range(1000000))
```

Also leverage:
- `map()` and `filter()` for clean transformations  
- `str.join()` instead of string concatenation  
- `itertools` for efficient iterators  

---

## 🔄 3. Optimize Loops with Comprehensions & Data Structures

Avoid manual loops when possible:

```python
# Using a loop
squares = []
for i in range(10000):
    squares.append(i*i)

# Better with list comprehension
squares = [i*i for i in range(10000)]
```

Use optimized data structures:
- ✅ `set` for fast lookups  
- ✅ `dict` for key-value mapping  
- ✅ `deque` for efficient queue/stack operations  

---

## 🧠 4. Cache Expensive Function Calls

Memoization = instant performance win for repeated or recursive logic:

```python
from functools import lru_cache

@lru_cache(maxsize=None)
def fib(n):
    if n < 2:
        return n
    return fib(n-1) + fib(n-2)

print(fib(100))
```

✅ `lru_cache` reduces recomputation overhead.

---

## 🧵 5. Leverage Concurrency (CPU or I/O)

Use **`multiprocessing`** for CPU-bound tasks:

```python
from multiprocessing import Pool

def square(n):
    return n * n

with Pool() as p:
    print(p.map(square, range(10)))
```

Use **`asyncio`** for I/O-heavy operations.

> Concurrency speeds up programs that wait on CPU or I/O.

---

## 📊 6. Use Optimized Libraries (NumPy, Pandas)

Vectorized operations are **orders of magnitude faster**:

```python
import numpy as np

# Native Python
nums = [i for i in range(1000000)]
squares = [i*i for i in nums]

# NumPy (faster)
arr = np.arange(1000000)
squares_np = arr * arr
```

Also explore `Pandas`, `scipy`, and `numexpr`.

---

## 🧪 7. Use JIT Compilers (Numba, PyPy, Cython)

Turn Python into compiled machine code with `Numba`:

```python
from numba import njit

@njit
def compute():
    total = 0
    for i in range(1000000):
        total += i
    return total

print(compute())
```

✅ Huge speed-ups with minimal code changes.

Also try:
- `PyPy` for general-purpose speed  
- `Cython` for writing C extensions in Python  

---

## 🏁 Final Thoughts

To boost Python speed:

✅ Profile first — optimize only what's slow  
✅ Use built-ins and vectorized ops  
✅ Add caching, concurrency, and JIT compilation where needed

Writing fast code doesn’t mean writing complex code. Small, focused changes deliver big wins. 🚀

---

**Happy coding, and may your functions always run fast! 🐍⚡**
