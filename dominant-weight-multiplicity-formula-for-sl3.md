# Dominant weight multiplicity formula for sl3

↑ **Parent:** [Sl3 interlacing character formula](sl3-interlacing-character-formula.md)

For the irreducible [highest-weight representation](highest-weight-representation.md) of the [special linear Lie algebra](special-linear-lie-algebra.md) $\mathfrak{sl}_3$ with [Dynkin labels](dynkin-label.md) $(a,b)$, let $(p,q)$ be a [dominant integral weight](dominant-integral-weight.md). Put $r=(2a+b-2p-q)/3$ and $s=(a+2b-p-2q)/3$. If these are not [integers](integer.md), the [weight multiplicity](weight-multiplicity.md) is zero; otherwise it is $\max\{0,1+\min(a,b,r,s)\}$.

To derive the formula, use the [sl3 interlacing character formula](sl3-interlacing-character-formula.md) with top row $(a+b,b,0)$. The target diagonal exponents are $(s+p+q,s+q,s)$, and an interlacing middle row $(P,Q)$ has $P+Q=2s+p+2q$, with bottom entry $s+p+q$. Thus

$$
\max\{b,2s+p+2q-b,s+p+q\}\leq P\leq\min\{a+b,2s+p+2q\}.
$$

Every integral $P$ in this interval gives exactly one [Gelfand–Tsetlin basis](gelfand-tsetlin-basis.md) vector. The upper bound minus the lower bound is the minimum of six differences: $a,s,r,r+p+q,b,s+q$. Since $p,q\geq0$, this minimum reduces to $\min(a,b,r,s)$. Counting the interval proves the formula, including absent [weights of a representation](weight-of-a-representation.md). This converts a two-dimensional [weight diagram](weight-diagram.md) calculation into four elementary boundary distances.

## ↑ Ancestors (11)

1. [Sl3 interlacing character formula](sl3-interlacing-character-formula.md)
2. [Formal character of a weight module](formal-character-of-a-weight-module.md)
3. [Highest-weight representation](highest-weight-representation.md)
4. [Semisimple Lie algebra](semisimple-lie-algebra-split.md)
5. [Lie algebra](lie-algebra-split.md)
6. [Lie theory](lie-theory-split.md)
7. [Diagonal dominance](diagonal-dominance.md)
8. [Algebra](algebra-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-52/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3/1/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-49/2/solution.md)
- [Shell multiplicities in an SU(3) weight diagram](shell-multiplicities-in-an-su-3-weight-diagram.md)
