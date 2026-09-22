<h1 id="6b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under the moving-coordinate transformation, the forcing is $H(y)$. Choose a stationary solution $U(s,y)=w(y)$, which requires precisely $w''+H=0$. The left spatial limit of $Ay+B$ is zero only if $A=B=0$. Therefore one solution is the [transported step forcing in an advection-diffusion equation](../../../../../../transported-step-forcing-in-an-advection-diffusion-equation.md) profile

$$
\boxed{u(t,x)=-\frac12(x-t)_+^2.}
$$

It has $u_t=(x-t)_+$ and $u_x=-(x-t)_+$, so their sum vanishes; almost everywhere $u_{xx}=-H(x-t)$, canceling the source. The first derivatives are continuous on the moving interface. For each fixed $t$, the profile is zero far to the left and tends to minus infinity to the right, as required. The PDE holds pointwise off that interface and weakly across it, consistently with the requested continuously differentiable regularity.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6B](../../6b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
