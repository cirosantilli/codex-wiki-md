<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $n_0=v(x)$ and $y_0=\pi^{-n_0}x\in R^\times$. Choose $a_{n_0}$ to represent the residue of $y_0$, and set $y_1=(y_0-a_{n_0})/\pi\in R$. Continue by choosing $a_{n_0+j}$ representing $y_j$ and putting $y_{j+1}=(y_j-a_{n_0+j})/\pi$. The first digit is not in $\mathfrak m$, because $y_0$ is a unit. After $r$ steps,

$$
x=\sum_{j=0}^{r-1}a_{n_0+j}\pi^{n_0+j}+\pi^{n_0+r}y_r.
$$

The error has valuation at least $n_0+r$, so the partial sums converge to the existing element $x$. This proves the [digit expansion in a discretely valued field](../../../../../../digit-expansion-in-a-discretely-valued-field.md) without any completeness assumption.

The leading exponent is forced to be $v(x)$. Reduction of $\pi^{-n_0}x$ modulo $\mathfrak m$ forces the first digit, and the recursive quotient then forces every later digit. Thus the expansion is unique for the chosen representatives. No assumption that the representative of the zero residue is literally zero is needed.

**Arbitrary series of this form need not converge in $K$.** Their partial sums are Cauchy, so they do converge if $K$ is complete. For a counterexample take $K=\mathbb Q$ with the three-adic valuation, $\pi=3$, and $A=\{0,1,2\}$. [Hensel lemma](../../../../../../hensel-s-lemma.md) applied to $T^2-10$ at the simple residue root $1$ gives a square root of $10$ in $\mathbb Q_3$. Its three-adic digits form such a series, but its sums cannot converge to an element of $\mathbb Q$, since that would give a rational square root of $10$. Convergence to an already given element and convergence of every possible digit sequence are different assertions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
