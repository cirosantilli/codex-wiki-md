<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $\varepsilon>0$. At an [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md), $w=\gamma v=f(v)$, so

$$
v\bigl[(a-v)(v-1)-\gamma\bigr]=0.
$$

The nonzero roots are

$$
v_\pm=\frac{1+a\pm\sqrt{(1-a)^2-4\gamma}}2,\qquad w_\pm=\gamma v_\pm.
$$

Consequently, with $\gamma_c=(1-a)^2/4$, there are three distinct [equilibria](../../../../equilibrium-point-of-a-dynamical-system.md) for $0<\gamma<\gamma_c$, two distinct [equilibria](../../../../equilibrium-point-of-a-dynamical-system.md) for $\gamma=\gamma_c$, and only the origin for $\gamma>\gamma_c$. At equality the two nonzero [equilibria](../../../../equilibrium-point-of-a-dynamical-system.md) coincide; for $0<\gamma<\gamma_c$ they both have $a<v<1$. Geometrically, $\gamma_c$ is the maximum of the concave quadratic $(a-v)(v-1)$.

Since $f'(0)=-a$, the [Jacobian matrix](../../../../jacobian-matrix.md) at the origin is

$$
J_0=\begin{pmatrix}-a/\varepsilon&-1/\varepsilon\\\gamma&-1\end{pmatrix},\qquad
\operatorname{tr}J_0=-\frac a\varepsilon-1<0,\qquad
\det J_0=\frac{a+\gamma}{\varepsilon}>0.
$$

Thus the origin is always [asymptotically stable](../../../../asymptotic-stability.md). Its [eigenvalues](../../../../eigenvalue.md) are

$$
\lambda_\pm=\frac{-(a+\varepsilon)\pm\sqrt{(a-\varepsilon)^2-4\varepsilon\gamma}}{2\varepsilon}.
$$

Writing $\gamma_N=(a-\varepsilon)^2/(4\varepsilon)$, the origin is a [stable node](../../../../stable-node.md) for $0<\gamma<\gamma_N$ and a [stable focus](../../../../stable-spiral.md) for $\gamma>\gamma_N$. At $\gamma=\gamma_N>0$ it is a [degenerate node](../../../../degenerate-node.md): the repeated negative [eigenvalue](../../../../eigenvalue.md) has only one independent [eigenvector](../../../../eigenvector.md), since the nonzero off-diagonal entry prevents $J_0$ being a scalar matrix. If $a=\varepsilon$, then $\gamma_N=0$ and every permitted $\gamma>0$ gives a [stable focus](../../../../stable-spiral.md). This change from node to focus does not change [stability](../../../../stability-of-a-numerical-method.md) and is not a [Hopf bifurcation](../../../../hopf-bifurcation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
