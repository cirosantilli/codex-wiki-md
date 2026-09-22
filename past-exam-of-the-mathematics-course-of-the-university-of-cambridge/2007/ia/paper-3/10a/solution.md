<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

The [divergence of a cross product](../../../../../divergence-of-a-cross-product.md) identity and the stated static field equations give

$$
\nabla\cdot(\mathbf E\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf B)=-\mathbf E\cdot\mathbf J.
$$

For an outward-oriented closed surface, the [divergence theorem](../../../../../divergence-theorem.md) therefore gives the flux of the specified [Poynting vector](../../../../../poynting-vector.md) normalization:

$$
\boxed{\iint_{\partial V}\mathbf P\cdot d\mathbf S=-\iiint_V\mathbf E\cdot\mathbf J\,dV.}
$$

No open-surface conclusion follows from this equation without including its closing pieces.

For the particular fields, direct calculation gives

$$
\mathbf J=\nabla\times\mathbf B=(0,-z,-y),\qquad\mathbf P=\mathbf E\times\mathbf B=(x^2y,-xz^2,-xyz),\qquad\nabla\cdot\mathbf P=xy.
$$

The fields also have $\nabla\times\mathbf E=0$, $\nabla\cdot\mathbf B=0$, and $\nabla\cdot\mathbf J=0$, consistently with the required equations. Close the outward spherical patch by the two planar half-disks on $x=0$ and $y=0$, forming the quarter unit ball $V$. Its total closed flux is

$$
\iiint_Vxy\,dV=\int_0^{\pi/2}\cos\varphi\sin\varphi\,d\varphi\int_0^1r^3dr\int_{-\sqrt{1-r^2}}^{\sqrt{1-r^2}}dz=\int_0^1r^3\sqrt{1-r^2}\,dr=\frac{2}{15},
$$

where $r$ in this integral is cylindrical radius. The $x=0$ face has outward normal $-\mathbf e_x$ and zero flux because $P_x=0$ there. The $y=0$ face has outward normal $-\mathbf e_y$, so its flux is

$$
\int_{-1}^1\int_0^{\sqrt{1-z^2}}xz^2\,dx\,dz=\frac12\int_{-1}^1z^2(1-z^2)dz=\frac{2}{15}.
$$

Subtracting these planar contributions from the closed flux gives the requested open-patch answer

$$
\boxed{\iint_{\text{spherical patch}}\mathbf P\cdot d\mathbf S=0.}
$$

As a direct check, on the unit sphere the outward normal is $(x,y,z)$ and $\mathbf P\cdot\mathbf n=xy(x^2-2z^2)$. With spherical angles $0\le\vartheta\le\pi$, $0\le\varphi\le\pi/2$, its [surface integral](../../../../../surface-integral.md) is $\frac14\int_0^\pi\sin^5\vartheta\,d\vartheta-\int_0^\pi\sin^3\vartheta\cos^2\vartheta\,d\vartheta=\frac14(16/15)-4/15=0$. The curved patch's vanishing flux is a cancellation, not an inference that its flux density vanishes everywhere.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
