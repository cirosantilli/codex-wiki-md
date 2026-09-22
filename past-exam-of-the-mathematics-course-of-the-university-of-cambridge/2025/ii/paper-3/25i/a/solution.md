<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a local parametrization $X(u^1,u^2)$, the [first fundamental form](../../../../../../first-fundamental-form.md) is the Euclidean inner product restricted to each tangent plane:

$$
I=g_{ij}\,du^i\,du^j,\qquad
g_{ij}=X_i\cdot X_j.
$$

Writing $u^1=u,u^2=v$, this is

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,
\qquad
E=X_u^2,\quad F=X_u\cdot X_v,\quad G=X_v^2.
$$

After choosing an orientation, the [Gauss map](../../../../../../gauss-map.md) is

$$
N=\frac{X_u\times X_v}{|X_u\times X_v|}.
$$

The [second fundamental form](../../../../../../second-fundamental-form-split.md) is $II(v,w)=\langle S(v),w\rangle$, where the shape operator is $S=-dN$. In coordinates,

$$
II=e\,du^2+2f\,du\,dv+g\,dv^2,
\qquad
e=N\cdot X_{uu},\quad
f=N\cdot X_{uv},\quad
g=N\cdot X_{vv}.
$$

The [Gaussian curvature](../../../../../../gaussian-curvature.md) and [mean curvature](../../../../../../mean-curvature.md) are respectively the determinant and half the trace of $S$:

$$
K=\frac{eg-f^2}{EG-F^2},
\qquad
H=\frac{eG-2fF+gE}{2(EG-F^2)}.
$$

Changing the chosen normal reverses $II$ and $H$ but leaves $K$ unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
