
## Commands

```bash
pip install -r requirements.txt
python -m memory_profiler run.py
```

## Sample Output

```
(venv) (base) ➜  python_memory_profiler git:(master) python -m memory_profiler run.py

Filename: run.py

Line #    Mem usage    Increment  Occurrences   Line Contents
=============================================================
     4     14.0 MiB     14.0 MiB           1   @profile
     5                                         def my_func():
     6     21.7 MiB      7.6 MiB           1       a = [1] * (10 ** 6)
     7    174.3 MiB    152.6 MiB           1       b = [2] * (2 * 10 ** 7)
     8   1659.0 MiB   1484.8 MiB           1       c = [3] * (2 * 10 ** 8)
     9   1502.8 MiB   -156.2 MiB           1       del b
    10   1502.8 MiB      0.0 MiB           1       return a
```

