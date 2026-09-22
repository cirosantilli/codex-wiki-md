<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use [trial division](../../../../../trial-division.md) on a shrinking residual. Once the trial divisor exceeds its [square root](../../../../../square-root.md), any residual larger than one is itself [prime](../../../../../prime-number-split.md).
```
PROCEDURE divisors(n: INTEGER): INTEGER;
VAR residual, trial, exponent, answer: INTEGER;
BEGIN
  residual := n; trial := 2; answer := 1;
  WHILE trial * trial <= residual DO
    exponent := 0;
    WHILE residual MOD trial = 0 DO
      residual := residual DIV trial;
      exponent := exponent + 1
    END;
    answer := answer * (exponent + 1);
    trial := trial + 1
  END;
  IF residual > 1 THEN answer := 2 * answer END;
  RETURN answer
END divisors;
```
For the outer [loop invariant](../../../../../loop-invariant.md), let $P$ be the set of [primes](../../../../../prime-number-split.md) below `trial` and $e_p$ their exponents in the original $n$. Then

$$
n=\mathrm{residual}\prod_{p\in P}p^{e_p},\qquad
\mathrm{answer}=\prod_{p\in P}(e_p+1),
$$

and `residual` has no [prime factor](../../../../../prime-factor.md) below `trial`. If `trial` divides the residual it must therefore be [prime](../../../../../prime-number-split.md): a composite trial value would have a smaller prime factor, contradicting this clause. If it does not divide, the zero exponent contributes the factor $1$.

For the inner [loop invariant](../../../../../loop-invariant.md), let $r_0$ be the residual on entry. Then $r_0=\mathrm{trial}^{\mathrm{exponent}}\mathrm{residual}$. Each exact division reduces the positive residual by at least a factor of two, so this loop terminates. At exit the exponent is the full multiplicity of `trial`; multiplying by `exponent+1` preserves the outer [loop invariant](../../../../../loop-invariant.md). The outer loop terminates because `trial` increases and `residual` never increases. When it exits, a composite residual would have a [prime factor](../../../../../prime-factor.md) at most its [square root](../../../../../square-root.md), yet every smaller trial factor has already been excluded. Hence the residual is $1$ or a single remaining [prime](../../../../../prime-number-split.md) of exponent $1$.

**The procedure computes $\tau(n)$ in $O(\sqrt n)$ unit-cost time and $O(1)$ auxiliary space**, with the separate successful divisions bounded by $\lfloor\log_2 n\rfloor$. No [array](../../../../../array-data-structure.md) or table of [primes](../../../../../prime-number-split.md) is needed, and $n=1$ correctly returns $1$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
