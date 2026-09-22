<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every $A\subseteq[n]$, define the [Walsh character](../../../../../../walsh-character.md)

$$
\chi_A(x)=(-1)^{\sum_{i\in A}x_i},
\qquad x\in\{0,1\}^n.
$$

These $2^n$ functions form an [orthonormal basis](../../../../../../orthonormal-basis.md). For the lazy walk, which stays put with probability $1/2$ and otherwise flips a uniformly chosen coordinate,

$$
P\chi_A=\left(1-\frac{|A|}{n}\right)\chi_A.
$$

Hence the eigenvalue $1-k/n$ has multiplicity $\binom nk$, for $0\leq k\leq n$.

The supplied [spectral upper bound for total variation mixing](../../../../../../spectral-upper-bound-for-total-variation-mixing.md) gives

$$
4\lVert P^t(x,\cdot)-\pi\rVert_{\mathrm{TV}}^2
\leq\sum_{k=1}^n\binom nk\left(1-\frac kn\right)^{2t}
\leq\left(1+e^{-2t/n}\right)^n-1
\leq e^{ne^{-2t/n}}-1.
$$

At $t=\tfrac12n\log n+Cn$, the last expression is $e^{e^{-2C}}-1$. Choosing $C=C(\varepsilon)$ so that this is at most $4\varepsilon^2$ proves

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)leq\frac12n\log n+C(\varepsilon)n.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
