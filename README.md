# Collaz conjecture
Given the computation
> a = n/2, if n = 0 (mod 2)
> 
> a = 3n + 1, if n = 1 (mod 2)

the Collaz conjucture states

> After many recurtions(treat a as new n, doing the computation), a approches 1, whatever integer n is chosen.

## Proof
There is no complete prove for the conjecture. Below lists some conclusions:
### Equilvalence
> Let a(n) denodes all a generates from an integer n by the recursion computaion,
> Collaz conjecture is equivalent to state that
> a(n) < n, after finite recursions
### Indefinite proof
> Many integers (of logarithmic density) satisfies the statement
### Verification
> Computers verify Collaz conjecture for integers up to 2<sup>68</sup>

# Discussion
Generalize the computaion as

> a = n/m, if n = 0 (mod m)
>
> a = p<sub>k</sub>n + q<sub>k</sub>, if n = k (mod m)

It's recognized that the rule#1 is in fact a modulo operation, and rule#k (k = 1, 2, ..., n-1) maps n into

> a = p<sub>k</sub>k + q<sub>k</sub> (mod m)

The Collaz conjecture may has something to do with the modulo operation. The recursions map a integer n into 0 (mod m), turning them into 1. Computor shows that, when the coefficients (p<sub>k</sub>, q<sub>k</sub>) satisfy

> p<sub>k</sub>k + q<sub>k</sub> = m, m<sup>2</sup>

the recursion converges. While they fails to converge while rhs is m<sup>3</sup>, m<sup>4</sup>, and so on.
Below lists some generalized computation, They could generate Collaz-like sequence {a(n)}  which converges into 1 :

> a = n/2, n = 0 (mod 2)
> 
> a = n + 1, n = 1 (mod 2)

> a = n/2, n = 0 (mod 2)
> 
> a = 3n + 1, n = 1 (mod 2)

> a = n/3, n = 0 (mod 3)
> 
> a = 2n + 1, n = 1 (mod 3)
> 
> a = n + 2, n = 2 (mod 3)

> a = n/3, n = 0 (mod 3)
> 
> a = 3n + 1, n = 1 (mod 3)
> 
> a = 2n + 2, n = 2 (mod 3)

> a = n/5, n = 0 (mod 5)
> 
> a = 4n + 1, n = 1 (mod 5)
> 
> a = 2n + 1, n = 2 (mod 5)
> 
> a = n + 2, n = 3 (mod 5)
> 
> a = n + 1, n = 4 (mod 5)

## [Demostration](http://tpcg.io/AXUAMK)
Visit the [online console here](http://tpcg.io/AXUAMK) for verification.
