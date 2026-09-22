<h1 id="6e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The class of $(1,1)$ is

$$
\{(\lambda,\lambda):\lambda\in(\mathbb Z/n\mathbb Z)^\times\},
$$

so its size is [Euler's totient function](../../../../../../euler-totient-function.md)

$$
\varphi(n)=n\prod_{p\mid n}\left(1-\frac1p\right).
$$

The unit group acts freely on every pair in $Y$: if $\lambda a\equiv a$ and $\lambda b\equiv b$, multiplying the [Bezout identity](../../../../../../bezout-identity.md) by $\lambda-1$ gives $\lambda\equiv1\pmod n$. Hence every equivalence class has size $\varphi(n)$. Dividing the answer from part (a) by this size gives

$$
\boxed{\frac{|Y|}{\varphi(n)}
=n\prod_{p\mid n}\frac{1-p^{-2}}{1-p^{-1}}
=n\prod_{p\mid n}\left(1+\frac1p\right)}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
