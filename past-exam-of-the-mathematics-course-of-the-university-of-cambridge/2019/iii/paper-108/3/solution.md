<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite measurable partition $\xi$,

$$
H_\mu(\xi)=-\sum_{A\in\xi}\mu(A)\log\mu(A).
$$

Its [conditional entropy of finite measurable partitions](../../../../../conditional-entropy-of-finite-measurable-partitions.md) relative to $\eta$ is

$$
H_\mu(\xi\mid\eta)
=\sum_{B\in\eta}\mu(B)
\left[-\sum_{A\in\xi}\mu(A\mid B)\log\mu(A\mid B)\right].
$$

The concavity of $-t\log t$, equivalently [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md), gives

$$
\boxed{H_\mu(\xi\mid\eta)\leq H_\mu(\xi).}
$$

The atoms of $T^{-1}\xi$ are $T^{-1}A$ with the same measures as the atoms $A$ of $\xi$. Hence $\boxed{H_\mu(T^{-1}\xi)=H_\mu(\xi)}$.

Set

$$
a_N=H_\mu\left(\bigvee_{n=0}^{N-1}T^{-n}\xi\right).
$$

The chain rule and invariance give $a_{N+M}\leq a_N+a_M$, so $(a_N)$ is a [subadditive sequence](../../../../../subadditive-sequence.md). Therefore

$$
h_\mu(T,\xi)=\lim_{N\to\infty}\frac{a_N}{N}
=\inf_{N\geq1}\frac{a_N}{N}.
$$

The [Kolmogorov-Sinai entropy](../../../../../kolmogorov-sinai-entropy.md) is $h_\mu(T)=\sup_\xi h_\mu(T,\xi)$ over finite partitions.

Taking $F=\{0,\ldots,N-1\}$ immediately shows that the infimum over arbitrary finite $F$ is at most $h_\mu(T,\xi)$. For the reverse inequality, apply [Shearer's inequality](../../../../../shearer-s-inequality.md) to translates of a fixed finite $F$ inside a long interval. Every interior coordinate is covered $|F|$ times, while only $O(\max F)$ boundary coordinates are lost. Subadditivity bounds the boundary contribution; division by the interval length and passage to the limit give

$$
h_\mu(T,\xi)\leq\frac1{|F|}H_\mu\left(\bigvee_{n\in F}T^{-n}\xi\right).
$$

Taking the infimum proves

$$
\boxed{h_\mu(T,\xi)=\inf_{\varnothing\ne F\subseteq\mathbb Z_{\geq0}\text{ finite}}
\frac1{|F|}H_\mu\left(\bigvee_{n\in F}T^{-n}\xi\right).}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
