<h1 id="33a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
\varepsilon=\mu-1,
\qquad
v=y-1,
\qquad
\dot\varepsilon=0.
$$

Then

$$
\begin{aligned}
\dot x&=x(\varepsilon-2v-v^2-2x^2),\\
\dot v&=-2v-x^2-vx^2-3v^2-v^3.
\end{aligned}
$$

The extended centre variables are $(x,\varepsilon)$ and the stable variable is $v$. Write the centre manifold as $v=h(x,\varepsilon)$. At quadratic order, the invariance equation

$$
h_x\dot x+h_\varepsilon\dot\varepsilon
=-2h-x^2-vx^2-3v^2-v^3
$$

gives

$$
h(x,\varepsilon)=-\frac{x^2}{2}+\text{higher-order terms}.
$$

Substitution into the $x$ equation gives the leading normal form

$$
\boxed{\dot x=\varepsilon x-x^3+\text{higher-order terms}.}
$$

This is a supercritical pitchfork: the $x=0$ branch loses stability as $\varepsilon$ becomes positive and stable branches $x=\pm\sqrt\varepsilon$ emerge. The original system is invariant under $x\mapsto-x$, so a pitchfork is exactly the symmetry-forced bifurcation expected. The physical quadrant $x\geq0$ displays its positive half.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33A](../../33a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
