<h1 id="24f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose first that $u$ is [harmonic](../../../../../../harmonic-function.md). Since

$$
\frac{\partial}{\partial y}u_x
=\frac{\partial}{\partial x}u_y
\quad\text{and}\quad
\frac{\partial}{\partial x}u_x
=-\frac{\partial}{\partial y}u_y,
$$

the [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) show that

$$
g:=u_x-iu_y
$$

is [holomorphic](../../../../../../holomorphic-function.md) on $D$. An open disc is a [simply connected domain](../../../../../../simply-connected-domain.md), so $g$ has a [holomorphic primitive](../../../../../../primitive-of-a-holomorphic-function-on-a-simply-connected-domain.md) $f$. If $f=p+iq$, then

$$
p_x=\operatorname{Re}f'=u_x,
\qquad
p_y=-\operatorname{Im}f'=u_y.
$$

Thus $p-u$ has zero [gradient](../../../../../../gradient.md) and is constant on the connected disc. Subtracting that real constant from $f$ gives

$$
\boxed{u=\operatorname{Re}f}.
$$

Conversely, if $u=\operatorname{Re}f$ for a holomorphic $f=u+iv$, differentiating the Cauchy-Riemann equations gives

$$
\Delta u=u_{xx}+u_{yy}=v_{yx}-v_{xy}=0.
$$

**Hence $u$ is harmonic. This proves the [harmonic function as the real part of a holomorphic function](../../../../../../harmonic-function-as-the-real-part-of-a-holomorphic-function.md) criterion on $D$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24F](../../24f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
