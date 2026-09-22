<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

A [bilinear form](../../../../../bilinear-form.md) $B$ on $V$ is [nondegenerate](../../../../../nondegenerate-bilinear-form.md) when

$$
B(v,w)=0\quad\text{for every }v\in V
\qquad\Longrightarrow\qquad w=0.
$$

In finite dimensions this is equivalent to nondegeneracy in the first argument.

Define the [linear map](../../../../../linear-map.md)

$$
\beta_1:V\longrightarrow V^*,
\qquad
\beta_1(w)=B_1(-,w).
$$

Nondegeneracy makes $\beta_1$ injective. Since $V$ and its [dual space](../../../../../dual-space.md) have the same finite dimension, $\beta_1$ is an isomorphism. Similarly define $\beta_2(w)=B_2(-,w)$ and set

$$
\boxed{\alpha=\beta_1^{-1}\beta_2}.
$$

Then $\alpha$ is linear and

$$
B_1(v,\alpha w)=\beta_1(\alpha w)(v)
=\beta_2(w)(v)=B_2(v,w).
$$

If $w\in\ker\alpha$, this identity gives $B_2(v,w)=0$ for every $v$. Conversely, if $B_2(v,w)=0$ for every $v$, then $B_1(v,\alpha w)=0$ for every $v$, so nondegeneracy gives $\alpha w=0$. Hence

$$
\boxed{\{w\in V:B_2(v,w)=0\text{ for every }v\in V\}=\ker\alpha}.
$$

This is the [representation of a bilinear form relative to a nondegenerate bilinear form](../../../../../representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form.md).

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
