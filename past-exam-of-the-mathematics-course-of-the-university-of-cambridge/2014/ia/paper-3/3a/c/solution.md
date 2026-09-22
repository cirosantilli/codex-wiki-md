<h1 id="3a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [divergence](../../../../../../divergence.md) formula reduces the problem to the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) $rf'+nf=0$ on $r>0$. Multiplication by $r^{n-1}$ makes it an exact derivative:

$$
\frac{d}{dr}(r^nf(r))=r^{n-1}(rf'(r)+nf(r))=0.
$$

Since the interval $r>0$ is connected, $r^nf(r)$ is a single constant $C$. Conversely, substituting $f=Cr^{-n}$ into the [divergence](../../../../../../divergence.md) formula gives zero. Thus

$$
\boxed{\mathbf F(\mathbf x)=C\,\frac{\mathbf x}{|\mathbf x|^n}\quad(\mathbf x\ne0).}
$$

This proves both existence and uniqueness up to the constant within the specified radial class. For $n=1$, the two punctured half-lines still share this same constant because the stipulated coefficient is one [function](../../../../../../function-split.md) of $r=|x|$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3A](../../3a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
