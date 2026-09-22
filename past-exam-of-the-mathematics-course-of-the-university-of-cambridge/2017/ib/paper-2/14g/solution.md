<h1 id="14g/solution">Solution</h1>

↑ **Parent:** [14G](../14g.md)

For unit $u$, put $A=I-2uu^T$. Then $A^T=A$ and $A^2=I$, so $A$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md). The affine [reflection in a hyperplane](../../../../../reflection-in-a-hyperplane.md) is $R(x)=Ax+2cu$. Hence $R(x)-R(y)=A(x-y)$ preserves the [Euclidean norm](../../../../../euclidean-norm.md) and distance, and $R(x)=x$ whenever $u\cdot x=c$. Thus it is an [Euclidean isometry](../../../../../euclidean-isometry.md) fixing the hyperplane pointwise.

For $p\ne q$, any reflection exchanging them must have normal parallel to $p-q$, and its fixed hyperplane must contain their midpoint. These requirements determine the perpendicular bisector uniquely:

$$
\boxed{u=\frac{p-q}{\|p-q\|},\qquad c=u\cdot\frac{p+q}{2},\qquad R(p)=q.}
$$

Changing both signs of $u,c$ leaves the same reflection. It belongs to the [orthogonal group](../../../../../orthogonal-group.md) $O(n)$ exactly when its translation term vanishes, that is, $c=0$. Since $c=(\|p\|^2-\|q\|^2)/(2\|p-q\|)$,

$$
\boxed{R\in O(n)\iff\|p\|=\|q\|.}
$$

To prove the [finite reflection decomposition of a Euclidean isometry](../../../../../finite-reflection-decomposition-of-a-euclidean-isometry.md), first note that a distance-preserving map $g$ fixing zero preserves inner products by the [polarization identity](../../../../../polarization-identity.md). Its values on an orthonormal basis $e_i$ form an orthonormal basis, and $g(x)\cdot g(e_i)=x_i$ shows $g(x)=\sum_i x_i g(e_i)$. Thus $g$ is orthogonal.

Every [orthogonal transformation](../../../../../orthogonal-transformation.md) is a product of at most $n$ linear reflections: if $g(e_1)\ne e_1$, reflect $g(e_1)$ to $e_1$ using the hyperplane normal $g(e_1)-e_1$, which passes through zero. The resulting orthogonal transformation fixes $e_1$, and its restriction to $e_1^\perp$ is handled inductively in dimension $n-1$. If $g(e_1)=e_1$, no initial reflection is necessary. Reflections on the complement extend by fixing $e_1$; the induction starts in dimension zero.

For an arbitrary isometry $f$, if $f(0)\ne0$, first reflect $f(0)$ to zero across its perpendicular bisector with zero. Composing this one affine reflection with $f$ gives an orthogonal transformation. If $f(0)=0$, skip the initial reflection. Therefore

$$
\boxed{f\text{ is a product of at most }n+1\text{ hyperplane reflections}.}
$$

The [glide reflection](../../../../../glide-reflection.md) $(x,y)\mapsto(x+1,-y)$ cannot use fewer than three: its determinant sign is negative, excluding zero or two reflections, while absence of fixed points excludes a single reflection. Three suffice by reflecting successively in $x=0$, $x=1/2$, and $y=0$.

## ↑ Ancestors (10)

1. [14G](../14g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
