<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

Put $b(v,w)=\varphi(w)(v)$. Each $\varphi(w)$ belongs to the [dual space](../../../../dual-space-split.md) $V'$, so it is a [linear functional](../../../../linear-functional.md). For [real numbers](../../../../real-number.md) $a,b_0$ and [vectors](../../../../vector.md) $v_1,v_2,w$, this gives

$$
b(av_1+b_0v_2,w)=\varphi(w)(av_1+b_0v_2)
=a\,b(v_1,w)+b_0b(v_2,w).
$$

The [linearity](../../../../linearity.md) of $\varphi$ gives [linearity](../../../../linearity.md) in the second argument as well:

$$
b(v,aw_1+b_0w_2)
=(a\varphi(w_1)+b_0\varphi(w_2))(v)
=a\,b(v,w_1)+b_0b(v,w_2).
$$

Thus **$b$ is a [bilinear form](../../../../bilinear-form-split.md)**.

Its [right radical of a bilinear form](../../../../right-radical-of-a-bilinear-form.md) is exactly $\ker\varphi$, because

$$
b(v,w)=0\text{ for every }v\in V
\ \Longleftrightarrow\ \varphi(w)=0.
$$

If $b$ is a [nondegenerate bilinear form](../../../../nondegenerate-bilinear-form.md), this [kernel](../../../../kernel-of-a-linear-map-split.md) is zero. Since $V$ is a [finite-dimensional vector space](../../../../finite-dimensional-vector-space.md) and $\dim V'=\dim V$, the [rank-nullity theorem](../../../../rank-nullity-theorem.md) makes $\varphi$ [surjective](../../../../surjective-function.md).

Conversely, if $\varphi$ is [surjective](../../../../surjective-function.md), the same [dimension](../../../../dimension-vector-space.md) equality makes it [injective](../../../../injective-function.md), so the [right radical](../../../../right-radical-of-a-bilinear-form.md) is zero. If $v$ lies in the [left radical](../../../../left-radical-of-a-bilinear-form.md), then $f(v)=0$ for every $f\in V'$, because every $f$ is some $\varphi(w)$. A nonzero $v$ can be included in a [basis](../../../../basis.md) and detected by its [coordinate functional](../../../../coordinate-functional.md), so this forces $v=0$. Both radicals vanish, proving

$$
\boxed{b\text{ is nondegenerate}\ \Longleftrightarrow\ \varphi\text{ is surjective}.}
$$

## ↑ Ancestors (12)

1. [a](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
