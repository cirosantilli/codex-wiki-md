<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First make the invertible linear change of [homogeneous coordinates](../../../../homogeneous-coordinate.md)

$$
U=-y,\qquad V=\sqrt3\,z,\qquad W=x.
$$

The original equation becomes

$$
V^2W=U^3-W^3=(U-W)(U-\omega W)(U-\omega^2W),
\qquad \omega=\exp(2\pi\mathrm i/3).
$$

This takes the [flex](../../../../inflection-point-of-an-algebraic-plane-curve.md) $[0:0:1]$ to the point at infinity $[0:1:0]$ of a [Weierstrass model](../../../../weierstrass-equation-of-an-elliptic-curve.md).

Put $h=\omega-1$ and choose $s\in\mathbb C$ with $s^2=h^3$. Both are nonzero. Define

$$
X=\frac{U-W}{h},\qquad Y=\frac V{s},\qquad Z=W.
$$

Since $U=hX+Z$, the three factors on the right are $hX$, $h(X-Z)$ and $h(X-\lambda Z)$, where

$$
\boxed{\lambda=\frac{\omega^2-1}{\omega-1}=1+\omega=\frac{1+\mathrm i\sqrt3}{2}.}
$$

The resulting equation is precisely

$$
\boxed{Y^2Z-X(X-Z)(X-\lambda Z)=0,}
$$

the [Legendre form of an elliptic curve](../../../../legendre-form-of-an-elliptic-curve.md). In particular, $\lambda\ne0,1$.

Combining the two changes gives an explicit [projective transformation](../../../../projective-linear-transformation.md) from the original coordinates:

$$
\begin{pmatrix}X\\Y\\Z\end{pmatrix}
=\begin{pmatrix}
-1/h&-1/h&0\\
0&0&\sqrt3/s\\
1&0&0
\end{pmatrix}
\begin{pmatrix}x\\y\\z\end{pmatrix}.
$$

Its [determinant](../../../../determinant.md) is $-\sqrt3/(hs)\ne0$, so this is a valid transformation of the whole [projective plane](../../../../projective-plane.md), including the points where an affine coordinate would be undefined.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
