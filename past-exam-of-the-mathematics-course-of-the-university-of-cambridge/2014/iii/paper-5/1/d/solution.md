<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [separable Hilbert space](../../../../../../separable-hilbert-space.md) has a countable subset dense in its [norm topology](../../../../../../norm-topology.md).

**The printed assertion about all [locally square-integrable functions](../../../../../../locally-square-integrable-function.md) is false.** The proposed average is not even finite for every such function: for $f(x)=x$,

$$
\frac1R\int_{-R}^R f(x)^2\,dx=\frac23R^2\longrightarrow\infty.
$$

It also fails positive definiteness. The nonzero function $f=\mathbf1_{[0,1]}$ has

$$
\lim_{R\to\infty}\frac1R\int_{-R}^R f(x)^2\,dx=0.
$$

Consequently this formula cannot define an [inner product](../../../../../../inner-product.md), much less a [Hilbert space](../../../../../../hilbert-space-split.md), on $L^2_{\mathrm{loc}}(\mathbb R)$.

A precise version of the intended nonseparability argument uses the [mean-square completion of trigonometric polynomials](../../../../../../mean-square-completion-of-trigonometric-polynomials.md). Start with the real vector space $V$ of finite linear combinations of $1$, $\cos(\lambda x)$, and $\sin(\lambda x)$, with arbitrary $\lambda>0$. Product-to-sum identities show that all the proposed cross averages exist. Distinct frequencies are [orthogonal](../../../../../../orthogonal-vectors.md), each sine and cosine has squared [norm](../../../../../../norm.md) one, and the constant function has squared [norm](../../../../../../norm.md) two. Thus, after collecting equal frequencies,

$$
\left\|a_0+\sum_j\bigl(a_j\cos(\lambda_j x)+b_j\sin(\lambda_j x)\bigr)\right\|^2
=2a_0^2+\sum_j(a_j^2+b_j^2).
$$

This is positive definite on $V$. Its [Hilbert space completion](../../../../../../hilbert-space-completion.md) $H$ contains the uncountable [orthonormal set](../../../../../../orthonormal-set.md) $\{\cos(\lambda x):\lambda>0\}$. The distance between two distinct members is $\sqrt2$. Their open balls of radius $1/2$ are pairwise disjoint, and a dense subset must meet each one. A countable dense subset is therefore impossible: **this corrected completed space is nonseparable.** Completion is an essential additional construction; it does not validate the printed claim about all of $L^2_{\mathrm{loc}}$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
