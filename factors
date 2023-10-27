#!/usr/bin/python3
"""Modules."""
import sys

def the_fact(fd):
    try:
        with open(fd) as file:
            for i in file:
                num = int(i.strip())
                fac = find_fac(num)
                printfa(num, fac)
    except FileNotFoundError:
        print("Not found file")

def find_fac(num):
    facs = []
    sq = int(num * 0.5) + 1
    for i in range(2, sq):
        if num % i == 0:
            facs.append(i)
    return facs

def printfa(num, fac):
    if len(fac) == 0:
        print(f"{num}={num}*{1}")
    else:
        qu = num // fac[0]
        print(f"{num}={qu}*{fac[0]}")

if len(sys.argv) != 2:
    print("please enter the file name")
else:
    fd = sys.argv[1]
    the_fact(fd)
