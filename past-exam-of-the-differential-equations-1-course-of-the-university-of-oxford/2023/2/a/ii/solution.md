<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At an [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), $x=-y^2$ and $x^2=a^2y$, so $y(y^3-a^2)=0$. With $d=|a|^{2/3}>0$, the two [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) and their [Jacobian matrix](../../../../../jacobian-matrix.md) are

$$
\boxed{(0,0),\qquad(-d^2,d),}\qquad
J(x,y)=\begin{pmatrix}2x&-a^2\\1&2y\end{pmatrix}.
$$

At $(-d^2,d)$, $\det J=-3a^2<0$. The [trace-determinant stability criterion](../../../../../trace-determinant-stability-criterion.md) therefore gives an unstable [saddle equilibrium](../../../../../saddle-equilibrium.md). At the origin, the [eigenvalues](../../../../../eigenvalue.md) are $\lambda=\pm i|a|$: its [linearization](../../../../../linearization.md) is a [center equilibrium](../../../../../center-equilibrium.md). The [linearization stability theorem](../../../../../linearization-stability-theorem.md) does not classify this [nonhyperbolic equilibrium](../../../../../nonhyperbolic-equilibrium.md) of the nonlinear system.

**Nonlinear classification.** In fact the answer depends on $|a|$:

$$
\boxed{\begin{array}{c|c}
0<|a|<1&\text{unstable weak focus at the origin}\\
|a|=1&\text{stable center at the origin}\\
|a|>1&\text{asymptotically stable weak focus at the origin}.
\end{array}}
$$

Here is an explicit derivation, rather than an inference from the imaginary [eigenvalues](../../../../../eigenvalue.md). When $a^2=1$, set $L=1-x+y$. Near the origin $L>0$, and the [first integral](../../../../../first-integral.md)

$$
H(x,y)=\frac{1+xy}{L}+\log L
$$

has

$$
H_x=\frac{x+y^2}{L^2},\qquad H_y=\frac{y-x^2}{L^2},\qquad
\frac{dH}{dt}=0,\qquad
H=1+\frac{x^2+y^2}{2}+O\bigl((x^2+y^2)^{3/2}\bigr).
$$

Its [Hessian matrix](../../../../../hessian-matrix.md) at the origin is the identity. Small level curves are closed ovals on which the [vector field](../../../../../vector-field.md) is nonzero, proving the [center equilibrium](../../../../../center-equilibrium.md) classification and [Lyapunov stability](../../../../../lyapunov-stability.md).

For $a^2\ne1$, a higher-order [Lyapunov function](../../../../../lyapunov-function.md) calculation settles the issue. Put $k=|a|$, $U=x$, $V=ky$, $\tau=kt$, $p=k^{-1}$ and $q=k^{-2}$. Then

$$
U_\tau=-V+pU^2,\qquad V_\tau=U+qV^2.
$$

Write $R^2=U^2+V^2$ and introduce the differential operators

$$
\mathcal L=-V\partial_U+U\partial_V,\qquad
\mathcal N=pU^2\partial_U+qV^2\partial_V.
$$

Successively cancel the terms of degrees three, four and five in the derivative of $R^2+H_3+H_4+H_5$, using these [homogeneous polynomials](../../../../../homogeneous-polynomial.md):

$$
\begin{aligned}
H_3&=-2pU^2V-\tfrac43pV^3+\tfrac43qU^3+2qUV^2,\\
H_4&=2p^2U^2V^2-4pq(U^3V+UV^3)+(p^2-q^2)V^4,\\
H_5&=-\tfrac{4q}{15}(p^2+8q^2)U^5
+\tfrac{16q}{3}(p^2-q^2)U^3V^2
-\tfrac{4p}{3}(p^2-q^2)U^2V^3\\
&\quad+4q(p^2-q^2)UV^4+\tfrac{4p}{15}(11q^2-2p^2)V^5.
\end{aligned}
$$

Direct differentiation verifies $\mathcal LH_3=-\mathcal N R^2$, $\mathcal LH_4=-\mathcal NH_3$ and $\mathcal LH_5=-\mathcal NH_4$. The remaining degree-six term has circular average

$$
c=\frac1{2\pi}\int_0^{2\pi}(\mathcal NH_5)(\cos\theta,\sin\theta)\,d\theta
=\frac{pq(q^2-p^2)}4=\frac{1-k^2}{4k^7}.
$$

For example, the only nonzero averages of degree-six monomials needed here are $\langle U^6\rangle=\langle V^6\rangle=5/16$ and $\langle U^4V^2\rangle=\langle U^2V^4\rangle=1/16$. Since $\mathcal L=\partial_\theta$ in [polar coordinates](../../../../../polar-coordinates.md), the zero-average part can be cancelled by a degree-six [homogeneous polynomial](../../../../../homogeneous-polynomial.md) $H_6$ satisfying

$$
\mathcal LH_6=cR^6-\mathcal NH_5.
$$

Indeed its restriction to the unit circle is obtained by integrating a zero-average trigonometric polynomial; its Fourier modes have orders $2,4,6$, so multiplication by $R^6$ gives a polynomial. Consequently the positive [Lyapunov function](../../../../../lyapunov-function.md) $W=R^2+H_3+H_4+H_5+H_6$ satisfies

$$
\frac{dW}{d\tau}=cR^6+O(R^7).
$$

For $k>1$ this is strictly negative near the origin, giving [asymptotic stability](../../../../../asymptotic-stability.md). For $k<1$ it is strictly positive, and $W_\tau\geq C W^3$ in a sufficiently small neighbourhood; every nonzero starting point must eventually leave that neighbourhood. Finally $\theta_\tau=1+O(R)>0$, so the nearby trajectories rotate: these are [weak foci](../../../../../weak-focus.md), with the stability stated above. Merely calling the nonlinear origin a center for every $a\ne0$ would miss this distinction.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
