#!/usr/bin/python3
import sys


def factorize(n):
    for i in range(2, int(n**0.5)+1):
        if n % i == 0:
            return (i, n // i)
    return (n, 1)


numbers = []
try:
    if len(sys.argv) > 1:
        with open(sys.argv[1], "r") as nf:
            try:
                numbers = [int(L) for L in nf.readlines()]
            except Exception:
                pass
except Exception:
    pass


for n in numbers:
    p, q = factorize(n)
    print(f"{n}= {p}*{q}")
