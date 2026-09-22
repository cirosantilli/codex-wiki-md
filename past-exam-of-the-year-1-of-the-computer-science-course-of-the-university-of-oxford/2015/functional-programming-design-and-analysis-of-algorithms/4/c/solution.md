<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the requested `Int`-typed operation, remove the first element as well as its later multiples:
```
sieve :: [Int] -> [Int]
sieve [] = []
sieve (p:xs) = [x | x <- xs, x `rem` p /= 0]
```
On its intended input, `p` is positive, so the [remainder](../../../../../remainder.md) is defined. An arbitrary list headed by zero lies outside this convention.

To enumerate literally all [prime numbers](../../../../../prime-number-split.md), use unbounded `Integer` arithmetic:
```
primes :: [Integer]
primes = go [2..]
  where
    go :: [Integer] -> [Integer]
    go [] = []
    go (p:xs) =
      p : go [x | x <- xs, x `rem` p /= 0]
```
At each stage, the smallest remaining number has no smaller [prime divisor](../../../../../prime-factor.md) and is therefore prime. Removing its larger multiples preserves every later prime and removes any [composite number](../../../../../composite-number.md) once its least [prime divisor](../../../../../prime-factor.md) is processed. [Lazy evaluation](../../../../../lazy-evaluation.md) makes each requested finite prefix available. This implements the given repeated-filtering form of the [sieve of Eratosthenes](../../../../../sieve-of-eratosthenes.md). A bounded `Int` stream can only cover representable values; `Integer` supplies the all-primes interpretation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
