<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [uniaxial extensional flow](../../../../../../uniaxial-extensional-flow.md)

$$
\mathbf u=\dot\epsilon(-x/2,-y/2,z),
$$

the [spin tensor](../../../../../../spin-tensor.md) vanishes and

$$
\dot{\boldsymbol\gamma}
=\operatorname{diag}(-\dot\epsilon,-\dot\epsilon,2\dot\epsilon).
$$

The flow is steady and homogeneous, so with $\xi=1$ the [Jaumann derivative](../../../../../../jaumann-derivative.md) of $\boldsymbol\alpha$ vanishes. The structure equation yields

$$
\boldsymbol\alpha=\frac{c_2}{c_1}\dot{\boldsymbol\gamma}.
$$

Writing $k=c_2/c_1$ and using  
$\dot{\boldsymbol\gamma}:\dot{\boldsymbol\gamma}=6\dot\epsilon^2$ gives

$$
\dot{\boldsymbol\gamma}\boldsymbol\alpha+
\boldsymbol\alpha\dot{\boldsymbol\gamma}
-\frac23(\boldsymbol\alpha:\dot{\boldsymbol\gamma})\mathbf I
=2k\dot\epsilon\,\dot{\boldsymbol\gamma}.
$$

Consequently

$$
\boldsymbol\tau
=\left(\eta_0+\frac{b_1c_2}{c_1}
+\frac{2b_2c_2}{c_1}\dot\epsilon\right)
\dot{\boldsymbol\gamma}.
$$

The [extensional viscosity](../../../../../../extensional-viscosity.md) is the tensile stress difference divided by $\dot\epsilon$:

$$
\boxed{
\eta_{\rm ext}
=\frac{\tau_{zz}-\tau_{xx}}{\dot\epsilon}
=3\left(\eta_0+\frac{b_1c_2}{c_1}
+\frac{2b_2c_2}{c_1}\dot\epsilon\right)}.
$$

For $b_2=0$ this is the constant

$$
\boxed{\eta_{\rm ext}=3\left(\eta_0+\frac{b_1c_2}{c_1}\right)}.
$$

The factor three is the [Trouton ratio](../../../../../../trouton-ratio.md) associated with the effective zero-rate shear viscosity.

## ↑ Ancestors (11)

1. [C](../c.md)
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
