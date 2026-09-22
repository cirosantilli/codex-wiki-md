<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau=T_r\wedge T_R$. The function $z\mapsto\log|z|$ is a [harmonic function](../../../../../../harmonic-function.md) on the annulus $r<|z|<R$, so [Itô formula](../../../../../../ito-s-lemma.md) shows that

$$
\log|B_{t\wedge\tau}|
$$

is a bounded [martingale](../../../../../../martingale-split.md). By the [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to this martingale,

$$
\log|x|
=\mathbb E_x[\log|B_\tau|]
=p\log r+(1-p)\log R,
$$

where $p=\mathbb P_x(T_r<T_R)$. Solving gives the [planar Brownian annulus hitting probability](../../../../../../planar-brownian-annulus-hitting-probability.md)

$$
\boxed{\mathbb P_x(T_r<T_R)
=\frac{\log R-\log|x|}{\log R-\log r}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
