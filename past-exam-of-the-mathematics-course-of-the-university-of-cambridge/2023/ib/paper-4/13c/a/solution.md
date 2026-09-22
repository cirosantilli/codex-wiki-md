<h1 id="13c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u\mapsto u+\varepsilon\eta$ and $v\mapsto v+\varepsilon\xi$, where the variations vanish on the boundary. The [first variation](../../../../../../first-variation.md) is

$$
\begin{aligned}
\delta\mathcal L
=\iint_\Omega \bigl(&f_u\eta+f_v\xi
+f_{u_x}\eta_x+f_{u_y}\eta_y\\
&+f_{v_x}\xi_x+f_{v_y}\xi_y)\,dx\,dy.
\end{aligned}
$$

Applying [integration by parts](../../../../../../integration-by-parts.md) to the four derivative terms and discarding the boundary contributions gives

$$
\delta\mathcal L=\iint_\Omega
\left(f_u-\frac{\partial f_{u_x}}{\partial x}
-\frac{\partial f_{u_y}}{\partial y}\right)\eta\,dx\,dy
$$



$$
{}+\iint_\Omega
\left(f_v-\frac{\partial f_{v_x}}{\partial x}
-\frac{\partial f_{v_y}}{\partial y}\right)\xi\,dx\,dy.
$$

The variations $\eta$ and $\xi$ are independent and arbitrary in the interior. The [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the two [Euler-Lagrange equations for two fields](../../../../../../euler-lagrange-equations-for-two-fields.md)

$$
\boxed{f_u-\partial_x f_{u_x}-\partial_y f_{u_y}=0},
$$



$$
\boxed{f_v-\partial_x f_{v_x}-\partial_y f_{v_y}=0}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13C](../../13c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
