<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $E:y^2=x^3+3$, direct counting gives

$$
\#E(\mathbb F_{17})=18,
\qquad
\#E(\mathbb F_{31})=43.
$$

Neither group order is divisible by $17$, so neither group contains a point of order $17$.

At $p=17$ the Frobenius trace is zero. The [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) has trace recurrence

$$
a_0=2,\quad a_1=0,\quad a_n=-17a_{n-2},
\qquad
\#E(\mathbb F_{17^n})=17^n+1-a_n.
$$

For every $n\geq1$, this order is congruent to one modulo $17$. Consequently $E(\mathbb F_{17^n})$ has no point of order $17$ for any $n$.

At $p=31$, the trace is $a=31+1-43=-11$. On $E[17]$, Frobenius has characteristic polynomial

$$
X^2+11X+31\equiv X^2+11X+14\pmod{17}.
$$

Its discriminant is $14$, a nonsquare in $\mathbb F_{17}$, so its two distinct eigenvalues lie in $\mathbb F_{17^2}^{\times}$. Their orders divide $17^2-1=288$, whence $\pi^{288}=1$ on $E[17]$. Thus all of $E[17]$ is rational over $\mathbb F_{31^{288}}$, and in particular a point of order $17$ exists over some extension with $n\geq2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
