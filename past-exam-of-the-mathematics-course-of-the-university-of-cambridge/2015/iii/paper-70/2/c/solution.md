<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Substitute part (b) into the spectral representation. The terms containing $\psi(ik)$ are

$$
\frac{i}{2\pi}\left[\left(\int_0^\infty-\int_0^{i\infty}\right)e^{ikz}(k-\gamma)\psi(ik)dk+\left(\int_0^{i\infty}-\int_0^{-\infty}\right)e^{ik(z-i\ell)}(k+\gamma)\psi(ik)dk\right].
$$

The transform $\psi(ik)$ is analytic for $\operatorname{Im}k>0$. Write $k=a+ib$. In the first quadrant,

$$
|e^{ikz}|=e^{-ay-bx},
$$

which decays since $x,y>0$. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) in that quadrant equates the two integrals in the first parentheses. In the second quadrant,

$$
|e^{ik(z-i\ell)}|=e^{-a(y-\ell)-bx},
$$

which decays since $a<0$, $b>0$, and $y<\ell$. The same [contour integration](../../../../../../contour-integration.md) equates the two integrals in the second parentheses. Therefore **$\psi(ik)$ makes no contribution**. This is [upper-quadrant cancellation of reflected boundary transforms](../../../../../../upper-quadrant-cancellation-of-reflected-boundary-transforms.md), and it uses the whole paired expression rather than attempting to discard an individual integral.

The terms involving $c$ cancel by the same two quadrant arguments with the analytic factors $k\pm\gamma$ and $\psi$ omitted. There is a sign defect in the printed reconstruction prefactor. The sides specified in part (a) form a clockwise boundary, so the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) gives a negative reconstruction sign. Indeed, integrating each spectral ray first yields $i/(z-\zeta)$, and hence the sum of the three ray integrals is $i\oint_{\mathrm{clockwise}}q_z(\zeta)/(z-\zeta)d\zeta=-2\pi q_z(z)$. Thus the printed positive prefactor reconstructs $-q_z$. The requested cancellation above holds with either overall sign, but the actual data-dependent derivative is

$$
\boxed{q_z=-\frac i\pi\left[-\int_0^\infty e^{ikz}(k-\gamma)\frac{H(k)}{D(k)}dk+\int_0^{i\infty}e^{ikz}H(k)dk+\int_0^{-\infty}e^{ikz+k\ell}(k+\gamma)\frac{H(k)}{D(k)}dk\right].}
$$

Decay at infinity fixes the integration constant when recovering $q$ from its [Wirtinger derivative](../../../../../../wirtinger-derivatives.md).

For completeness, the missing condition at infinity and the unrestricted printed $\gamma$ deserve an explicit [solvability of a decaying Robin strip](../../../../../../solvability-of-a-decaying-robin-strip.md) check. Let $Y_n$ be orthonormal [eigenfunctions](../../../../../../eigenfunction.md) from a [Sturm-Liouville problem](../../../../../../sturm-liouville-problem.md) of $-d^2/dy^2$ with $Y_n'(0)=\gamma Y_n(0)$ and $Y_n'(\ell)=-\gamma Y_n(\ell)$, and eigenvalues $\lambda_n$. With $g_n=\int_0^\ell gY_n\,dy$, [separation of variables](../../../../../../separation-of-variables.md) gives

$$
q(x,y)=-\sum_{\lambda_n>0}\frac{g_n}{\sqrt{\lambda_n}}e^{-\sqrt{\lambda_n}x}Y_n(y),\qquad g_n=0\ \text{required whenever }\lambda_n\leq0.
$$

Indeed, each coefficient obeys $q_n''-\lambda_nq_n=0$ and $q_n'(0)=g_n$. A positive eigenvalue has one decaying exponential; a zero eigenvalue has only affine solutions and a negative eigenvalue only oscillatory solutions, neither of which decays unless its coefficient vanishes. This also proves uniqueness in the decay class and justifies reflection symmetry there. For $\gamma>0$, all eigenvalues are positive. For $\gamma=0$, the constant eigenfunction requires $\int_0^\ell g\,dy=0$; the apparent zero of $D$ at the origin is then removable. For $\gamma<0$, compatibility with every nonpositive eigenmode is necessary. These restrictions cannot be inferred from smoothness and reflection symmetry alone. The printed [boundary value problem](../../../../../../boundary-value-problem.md) without any far-field condition permits additional growing or nondecaying homogeneous solutions, whereas the spectral transforms select the decaying branch.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
