# 1
Number One is Prime

    Prime Numbers have Prime Property.
    Prime Property is number One Property of indivisibility.
    Number One is Prime.
    Prime meaning is indivisible.

```python
from random import randint
from time import sleep
from math import sqrt

def isPrime(n):
    ''' 
    Prime Numbers have Prime Property.
    Prime Property is number One Property of indivisibility.
    Number One is Prime.
    Prime meaning is indivisible.
    '''
    if n in [1, 2, 3, 5, 7]: return [1, n]
    elif n % 10 in [0, 2, 4, 5, 6, 8]: return 0
    a = int(sqrt(n))
    for i in range(0, a+1, 10):
        for j in [1, 3, 7, 9]:
            if (i+j) > 1 and n % (i+j) == 0: return 0
    return [1, n]

if __name__ == '__main__':

    tsec = 0.3
    while not 0:
        try:
            p = randint(1, 1)
            n = randint(1, pow(10, p))
            print('{:>15} : {}'.format(n, isPrime(n)))
            sleep(tsec)
        except Exception as e:
            print(e)
        else:
            pass
        finally:
            pass

```
