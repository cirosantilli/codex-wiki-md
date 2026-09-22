<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The shear stress decreases monotonically from the fibre to zero at the free surface, so its maximum is

$$
\tau_{rz}(a)=\frac{\Delta p}{2L}\frac{b^2-a^2}{a}.
$$

Flow occurs precisely when this exceeds the yield stress:

$$
\boxed{\Delta p>\frac{2La\sigma_y}{b^2-a^2}.}
$$

When this condition holds, there is one [yield surface](../../../../../../yield-surface.md) $r=r_y$ determined by

$$
\frac G2\left(\frac{b^2}{r_y}-r_y\right)=\sigma_y.
$$

The region $a\leq r<r_y$ is yielded and the outer region $r_y\leq r\leq b$ is an unyielded [plug flow of a yield-stress fluid](../../../../../../plug-flow-of-a-yield-stress-fluid.md). In the yielded region, $du/dr=(\tau_{rz}-\sigma_y)/\eta$. The no-slip condition $u(a)=0$ gives

$$
u(r)=\frac1\eta\left[
\frac G2\left\{b^2\log\frac ra-\frac{r^2-a^2}{2}\right\}
-\sigma_y(r-a)
\right],
\qquad a\leq r\leq r_y.
$$

The unyielded layer translates without shearing at the plug speed

$$
\boxed{u_p=u(r_y)=\frac1\eta\left[
\frac G2\left\{b^2\log\frac{r_y}{a}-\frac{r_y^2-a^2}{2}\right\}
-\sigma_y(r_y-a)
\right].}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
