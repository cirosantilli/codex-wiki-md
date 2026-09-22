<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $u=F_N/\gamma_N$, where the Gaussian density is strictly positive. Extend $u\log u$ continuously at zero by $0\log0=0$. Both densities have [integral](../../../../../../integral.md) one, so the [relative entropy](../../../../../../kullback-leibler-divergence.md) can be written as

$$
 \begin{aligned}
 H_N(F_N)&=\int_{\mathbb R^N}\gamma_N u\log u\,d\mathbf v\\
 &=\int_{\mathbb R^N}\gamma_N(u\log u-u+1)\,d\mathbf v.
 \end{aligned}
$$

The bracket is nonnegative and vanishes only at $u=1$: its derivative for $u>0$ is $\log u$, with a unique minimum at one. Hence

$$
 \boxed{H_N(F_N)\geq0,\qquad H_N(F_N)=0\ \Longleftrightarrow\ F_N=\gamma_N\ \text{a.e.}}
$$

The inequality holds also for infinite entropy. Its negative integrand part is integrable, since $u\log u\geq-1/e$ and $\gamma_N$ has [integral](../../../../../../integral.md) one, so the extended-value [integral](../../../../../../integral.md) is well defined. This is [relative entropy in Kac's model](../../../../../../relative-entropy-in-kac-s-model.md); no differentiation is needed for nonnegativity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
