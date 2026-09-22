<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\beta=\mu[A]+\mu[B]$ and $\gamma=\mu[A+B]$, where all three [matrices](../../../../../../matrix.md) are symmetric. Submultiplicativity and the triangle inequality give

$$
\|[e^{xB},A]e^{xA}\|_2
\leq2\|A\|_2e^{x(\mu[A]+\mu[B])},
$$

and similarly the other [commutator](../../../../../../commutator.md) term is bounded by $2\|B\|_2e^{x\beta}$. Apply part (a) also to $A+B$ in the integral from part (b). The outer factor one-half cancels these twos, leaving

$$
\|F(t)-e^{t(A+B)}\|_2
\leq(\|A\|_2+\|B\|_2)\int_0^t e^{(t-x)\gamma+x\beta}\,dx.
$$

The [exponential divided difference](../../../../../../exponential-divided-difference.md) evaluates this integral. Thus

$$
\boxed{\|F(t)-e^{t(A+B)}\|_2\leq
(\|A\|_2+\|B\|_2)
\frac{e^{t\beta}-e^{t\gamma}}{\beta-\gamma}}
$$

when $\beta\ne\gamma$, and

$$
\boxed{\|F(t)-e^{t(A+B)}\|_2\leq
(\|A\|_2+\|B\|_2)\,te^{t\gamma}}
$$

when they coincide. The second expression is both the direct equal-exponent integral and the continuous limit of the first. The [Rayleigh-Ritz variational principle](../../../../../../rayleigh-ritz-variational-principle.md) also gives $\gamma\leq\beta$, although the integral computation does not require a strict inequality. These are valid coarse norm bounds; the cancellation between the two products can make the actual small-step error substantially smaller.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
