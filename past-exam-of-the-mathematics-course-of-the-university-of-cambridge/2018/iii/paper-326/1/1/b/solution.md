<h1 id="1/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The map $K^*K$ is a [bounded linear operator](../../../../../../../continuous-linear-operator.md), so the inverse image of the closed singleton $\{K^*f\}$ is closed. That inverse image is also a [convex set](../../../../../../../convex-set.md): if $K^*Ku=K^*Kv=K^*f$, every convex combination has the same image.

The identity $\mathcal N(K^*)=\mathcal R(K)^\perp$ gives

$$
K^*Ku=K^*f\quad\Longleftrightarrow\quad f-Ku\in\mathcal R(K)^\perp.
$$

Consequently such a $u$ exists exactly when $f$ is the sum of an element of $\mathcal R(K)$ and one of its [orthogonal complement](../../../../../../../orthogonal-complement.md). Thus

$$
\boxed{\mathbb L\neq\varnothing\ \Longleftrightarrow\
f\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

These are precisely the [least-squares solutions](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md). Indeed, if $r=Ku-f$ and $K^*r=0$, then for every $h$ the [Pythagorean identity](../../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|K(u+h)-f\|^2=\|r\|^2+\|Kh\|^2\geq\|r\|^2.
$$

Conversely, differentiating the squared residual along any real direction $h$ forces $\operatorname{Re}\langle K^*r,h\rangle=0$, hence the [normal equation for a linear inverse problem](../../../../../../../normal-equation-for-a-linear-inverse-problem.md). For any $u_*\in\mathbb L$, the difference of two solutions of the [normal equation for a linear inverse problem](../../../../../../../normal-equation-for-a-linear-inverse-problem.md) lies in $\mathcal N(K)$, since $\langle K^*Kh,h\rangle=\|Kh\|^2$. Therefore

$$
\boxed{\mathbb L=u_*+\mathcal N(K),}
$$

a closed [affine subspace](../../../../../../../affine-subspace.md); the empty case is closed and [convex](../../../../../../../convex-function.md) as well.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
