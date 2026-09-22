<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume all [partial derivatives](../../../../../../partial-derivative.md) needed below are continuous. The [multivariable chain rule](../../../../../../multivariable-chain-rule.md) is

$$
\boxed{f_x=g_uu_x+g_vv_x,}
$$

where the [partial derivatives](../../../../../../partial-derivative.md) of $g$ are evaluated at $(u(x,y),v(x,y))$. Apply the [product rule](../../../../../../product-rule.md) and the [multivariable chain rule](../../../../../../multivariable-chain-rule.md) once more:

$$
\begin{aligned}
f_{xx}&=(g_{uu}u_x+g_{uv}v_x)u_x+g_uu_{xx}\\
&\quad +(g_{vu}u_x+g_{vv}v_x)v_x+g_vv_{xx}.
\end{aligned}
$$

[Clairaut's theorem](../../../../../../symmetry-of-second-derivatives.md) gives $g_{vu}=g_{uv}$, so

$$
\boxed{f_{xx}=g_uu_{xx}+g_vv_{xx}+g_{uu}u_x^2+2g_{uv}u_xv_x+g_{vv}v_x^2.}
$$

Differentiating $f_x$ with respect to $y$ instead gives

$$
\boxed{f_{xy}=g_uu_{xy}+g_vv_{xy}+g_{uu}u_xu_y+g_{uv}(u_xv_y+v_xu_y)+g_{vv}v_xv_y.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
