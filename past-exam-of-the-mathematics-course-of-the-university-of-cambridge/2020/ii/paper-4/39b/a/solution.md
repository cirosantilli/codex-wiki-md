<h1 id="39b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The one-dimensional [Isentropic Euler equations](../../../../../../isentropic-euler-equations.md) are

$$
\rho_t+u\rho_x+\rho u_x=0,
\qquad
u_t+uu_x+\frac{c^2}{\rho}\rho_x=0,
\qquad
c^2=\frac{dp}{d\rho}.
$$

Define the [Riemann invariants for one-dimensional isentropic flow](../../../../../../riemann-invariants-for-one-dimensional-isentropic-flow.md)

$$
\boxed{R_\pm=u\pm\int_{\rho_0}^{\rho}\frac{c(s)}s\,ds}.
$$

Combining the two equations directly gives

$$
\boxed{\left[\partial_t+(u\pm c)\partial_x\right]R_\pm=0},
$$

so $R_\pm$ is constant on the corresponding [characteristic curve](../../../../../../characteristic-curve.md) $dx/dt=u\pm c$.

Initially both invariant disturbances are supported in $0\leq x\leq L$. Once the two characteristic families have separated, the left-moving packet is a [simple wave](../../../../../../simple-wave.md) with $R_+$ at its equilibrium value, while the right-moving packet is a [simple wave](../../../../../../simple-wave.md) with $R_-$ at equilibrium. Between and outside them, both invariants retain their equilibrium values. The schematic [spacetime diagram](../../../../../../spacetime-diagram.md) below uses the equilibrium slopes $\pm c_0$ and shows separation after $t=L/(2c_0)$.

<a id="39b/a/image-characteristic-curves-and-simple-wave-separation"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4-simple-wave-separation.png)

**[Figure 1](#39b/a/image-characteristic-curves-and-simple-wave-separation). Characteristic curves and simple-wave separation**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39B](../../39b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
