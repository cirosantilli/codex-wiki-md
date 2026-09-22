<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At order $\alpha^0$, the preceding equations give

$$
\boxed{\tau_{xy}^0=\eta g,
\qquad \tau_{xx}^0=2\eta\lambda g^2,
\qquad \tau_{yy}^0=\tau_{zz}^0=0}.
$$

At order $\alpha^1$, the quadratic term is evaluated on $\boldsymbol\tau^0$. Solving first the $yy$ equation, then $xy$, then $xx$, gives

$$
\boxed{\tau_{yy}^1=-\eta\lambda g^2,
\qquad
\tau_{xy}^1=-3\eta\lambda^2g^3},
$$



$$
\boxed{\tau_{xx}^1
=-\eta\lambda g^2-10\eta\lambda^3g^4,
\qquad \tau_{zz}^1=0}.
$$

Thus the apparent [shear viscosity](../../../../../../dynamic-viscosity.md) is

$$
\boxed{\eta_{\rm app}(g)=\frac{\tau_{xy}}g
=\eta\left[1-3\alpha(\lambda g)^2\right]
+O(\alpha^2)},
$$

so positive $\alpha$ produces [shear thinning](../../../../../../shear-thinning.md). The expansion requires $\alpha\ll1$ and $\alpha(\lambda g)^2\ll1$; it cannot describe arbitrarily high shear rates even when $\alpha$ is numerically small.

Using the [normal-stress difference](../../../../../../normal-stress-difference.md) definitions

$$
N_1=\tau_{xx}-\tau_{yy}=\Psi_1g^2,
\qquad
N_2=\tau_{yy}-\tau_{zz}=\Psi_2g^2,
$$

we find

$$
\boxed{\Psi_1
=2\eta\lambda\left[1-5\alpha(\lambda g)^2\right]
+O(\alpha^2),
\qquad
\Psi_2=-\alpha\eta\lambda+O(\alpha^2)}.
$$

In the low-rate limit, $-2\Psi_2/\Psi_1=\alpha+O(\alpha^2)$. A cone-and-plate or parallel-plate rheometer can measure shear stress and normal thrust over a low-rate range; combining $\Psi_1$ and $\Psi_2$ then estimates $\alpha$ independently of the viscosity scale.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
