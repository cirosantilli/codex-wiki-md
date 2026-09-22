<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The objective is [continuous](../../../../../continuous-function.md) on the compact disk, so a [global maximum](../../../../../global-maximum.md) exists. Its [gradient](../../../../../gradient.md) is $(e^x,2e^{2y})$, which is never zero, so a maximum cannot lie in the interior. It must have $x^2+y^2=1$.

Both coordinates of a maximizing point are positive. Reflecting a negative coordinate to its positive counterpart strictly increases the objective without changing the constraint; at an endpoint with one coordinate zero, a small move along the circle into the positive quadrant also increases the objective to first order. Thus it suffices to consider $x>0,y>0$.

The boundary [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are $e^x=2\lambda x$ and $2e^{2y}=2\lambda y$. Eliminate $\lambda$ to obtain the two-dimensional nonlinear [system of equations](../../../../../system-of-equations.md)

$$
\boxed{F(x,y)=
\begin{pmatrix}x^2+y^2-1\\ y e^x-2x e^{2y}\end{pmatrix}=0,
\qquad x>0,\ y>0.}
$$

Keeping this quadrant restriction excludes the boundary minimum that an unconstrained elimination could also produce. Under the stated uniqueness assumption for the admissible solution, the [global maximum](../../../../../global-maximum.md) must be that solution. Approximate it with [multivariable Newton iteration](../../../../../multivariable-newton-iteration.md), solving $J_F(z_n)\Delta_n=-F(z_n)$ and setting $z_{n+1}=z_n+\Delta_n$, with a suitable safeguard if needed. For example its explicit [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J_F(x,y)=\begin{pmatrix}
2x&2y\\
y e^x-2e^{2y}&e^x-4x e^{2y}
\end{pmatrix}.
$$

No numerical solution of the system is required.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
