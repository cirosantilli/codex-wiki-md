<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a generic saddle-focus [homoclinic orbit](../../../../../../homoclinic-orbit.md) at $\mu=0$, a smooth nondegenerate global reinjection along the selected unstable branch, and a sufficiently small neighborhood in which the linearized local flow supplies the leading passage map. Use linearizing coordinates if available; otherwise the calculation is a leading local approximation, not an exact consequence of [eigenvalues](../../../../../../eigenvalue.md) alone. Choose the incoming section near $(\rho,0,0)$ in the plane $y=0$, with coordinates $(\xi,z)$ where $r=\rho+\xi$ and $\rho>0$. This section is transverse since $\dot y=\omega r\ne0$. Choose an outgoing section $z=z_0>0$. We mark one return after a global excursion; intermediate crossings of $y=0$ during the spiral are not counted as separate global returns.

In cylindrical coordinates the local [flow](../../../../../../flow.md) is

$$
\dot r=\lambda_-r,\qquad\dot\theta=\omega,\qquad\dot z=\lambda_+z.
$$

For $0<z\ll z_0$, the time to the outgoing section is $t_\ell=\lambda_+^{-1}\log(z_0/z)$. Set $\delta=-\lambda_-/\lambda_+>0$ and $\Omega=\omega/\lambda_+$. The outgoing coordinates are

$$
\binom{X}{Y}=(\rho+\xi)\left(\frac z{z_0}\right)^\delta
\binom{\cos\vartheta}{\sin\vartheta},\qquad
\vartheta=\Omega\log\left(\frac{z_0}z\right).
$$

The global part of the [Poincaré return map](../../../../../../poincare-map.md) is smooth around $(X,Y)=(0,0)$ and takes the unstable-manifold point to $(\xi',z')=(0,-\mu)$. Expand it as

$$
\binom{\xi'}{z'}=\binom0{-\mu}
+\begin{pmatrix}a&b\\c&d\end{pmatrix}\binom XY
+O(X^2+Y^2),
$$

where the coefficients may depend smoothly on $\mu$ and the matrix is generically nonsingular. Absorbing the fixed $z_0^{-\delta}$ into them gives **the leading two-dimensional return map**

$$
\boxed{\begin{aligned}
\xi'&=(\rho+\xi)z^\delta(a\cos\vartheta+b\sin\vartheta)+O(z^{2\delta}),\\
z'&=-\mu+(\rho+\xi)z^\delta(c\cos\vartheta+d\sin\vartheta)+O(z^{2\delta}).
\end{aligned}}
$$

The remainder refers to the smooth global-map Taylor approximation with bounded $\xi$; corrections to the local linear approximation are also neglected. The global map supplies the additive splitting parameter and the local map supplies the power and logarithmic rotation. For an iterated excursion on this same unstable branch, the next coordinate must again satisfy $z'>0$. A nonpositive image leaves this local return domain; the formula must not be iterated through negative logarithms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
