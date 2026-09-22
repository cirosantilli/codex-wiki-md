<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [velocity gradient](../../../../../../velocity-gradient.md) as

$$
\mathbf L=\nabla\mathbf u
=\frac12\dot{\boldsymbol\gamma}+\boldsymbol\Omega,
$$

where $\boldsymbol\Omega$ is the [spin tensor](../../../../../../spin-tensor.md). Expanding the [upper-convected derivative](../../../../../../upper-convected-derivative.md) in the structure equation gives

$$
\frac{D\boldsymbol\alpha}{Dt}
-\boldsymbol\Omega\boldsymbol\alpha
+\boldsymbol\alpha\boldsymbol\Omega
+\frac{\xi-1}{2}
\left(\dot{\boldsymbol\gamma}\boldsymbol\alpha+
\boldsymbol\alpha\dot{\boldsymbol\gamma}\right)
+c_1\boldsymbol\alpha
=c_2\dot{\boldsymbol\gamma}.
$$

For $\xi=0$, the first four terms reproduce the upper-convected derivative. Setting

$$
\boxed{\xi=0,\qquad b_2=0}
$$

therefore gives

$$
\boldsymbol\tau=\eta_0\dot{\boldsymbol\gamma}+b_1\boldsymbol\alpha,
\qquad
\boldsymbol\alpha^{\triangledown}+c_1\boldsymbol\alpha
=c_2\dot{\boldsymbol\gamma}.
$$

With polymeric stress $\boldsymbol\tau_p=b_1\boldsymbol\alpha$, this is the [Oldroyd-B model](../../../../../../oldroyd-b-model.md). For $c_1>0$, its relaxation time and polymer viscosity are

$$
\lambda=\frac1{c_1},
\qquad
\eta_p=\frac{b_1c_2}{c_1}.
$$

Indeed the total stress obeys

$$
\boxed{
\boldsymbol\tau+\lambda\boldsymbol\tau^{\triangledown}
=(\eta_0+\eta_p)\dot{\boldsymbol\gamma}
+\lambda\eta_0\dot{\boldsymbol\gamma}^{\triangledown}}.
$$

For $\xi=2$, the coefficient of  
$\dot{\boldsymbol\gamma}\boldsymbol\alpha+
\boldsymbol\alpha\dot{\boldsymbol\gamma}$  
is $+1/2$, so the objective derivative becomes the [lower-convected derivative](../../../../../../lower-convected-derivative.md). Hence

$$
\boxed{\xi=2,\qquad b_2=0}
$$

recovers the [Oldroyd-A model](../../../../../../oldroyd-a-model.md), again with $c_1>0$ for a finite positive relaxation time. Parameter choices such as $b_1c_2=0$ give the degenerate Newtonian limit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
