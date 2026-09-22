<h1 id="11f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Summing the geometric series for the offspring [probability generating function](../../../../../../probability-generating-function.md) gives

$$
F_1(s)=\sum_{k=0}^\infty\frac{s^k}{2^{k+1}}=\frac1{2-s}.
$$

The fixed-point equation $s=1/(2-s)$ is $(s-1)^2=0$, whose only root in $[0,1]$ is one. The [Galton-Watson extinction fixed point](../../../../../../galton-watson-extinction-fixed-point.md) result therefore proves **extinction is certain**.

For the explicit iterates, the proposed formula at $n=1$ is $1/(2-s)$, so the base case holds. If it holds at $n$, part (a) gives

$$
F_{n+1}(s)=
\frac{n-(n-1)/(2-s)}{n+1-n/(2-s)}
=\frac{(n+1)-ns}{(n+2)-(n+1)s}.
$$

This is exactly the same formula with $n$ replaced by $n+1$. By induction,

$$
\boxed{F_n(s)=\frac{n-(n-1)s}{(n+1)-ns},\qquad n\geq1.}
$$

Evaluating the [probability generating function](../../../../../../probability-generating-function.md) at zero selects the mass of an empty generation:

$$
\boxed{P(X_n=0)=F_n(0)=\frac n{n+1}.}
$$

These [probabilities](../../../../../../probability.md) increase to one, also confirming the extinction conclusion directly.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
