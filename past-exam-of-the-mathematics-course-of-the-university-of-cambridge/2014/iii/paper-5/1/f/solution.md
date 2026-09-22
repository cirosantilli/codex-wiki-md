<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) states that every bounded [linear functional](../../../../../../linear-functional.md) $L$ on a real or complex [Hilbert space](../../../../../../hilbert-space-split.md) $H$ is represented by a unique $h\in H$:

$$
\boxed{L(v)=\langle v,h\rangle\quad(v\in H),\qquad\|L\|=\|h\|.}
$$

For the complex case take the [inner product](../../../../../../inner-product.md) to be linear in its first argument.

If $L=0$, choose $h=0$. Otherwise its [kernel](../../../../../../kernel-of-a-linear-map.md) $K$ is a closed linear subspace. Choose $x$ with $L(x)\ne0$ and let $z=x-P_Kx$, using the [orthogonal projection](../../../../../../orthogonal-projection.md). Then $z\ne0$, $z\perp K$, and $L(z)=L(x)\ne0$. For every $v$,

$$
v-\frac{L(v)}{L(z)}z\in K,
\qquad
\langle v,z\rangle=\frac{L(v)}{L(z)}\|z\|^2.
$$

Therefore take $h=L(z)z/\|z\|^2$ in the real case, and $h=\overline{L(z)}z/\|z\|^2$ in the complex case. The conjugate in the latter formula compensates for conjugate linearity in the second argument.

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|L(v)|\leq\|v\|\|h\|$, and evaluation at $v=h/\|h\|$ when $h\ne0$ gives equality of the [norms](../../../../../../norm.md). If two vectors represent $L$, their difference is [orthogonal](../../../../../../orthogonal-vectors.md) to every vector, including itself, hence zero. This proves all assertions of the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md).

## ↑ Ancestors (11)

1. [F](../f.md)
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
