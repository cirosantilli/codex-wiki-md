<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First suppose $u$ is a classical [harmonic function](../../../../../../harmonic-function.md). At a local maximum of $u-v$, its [Hessian matrix](../../../../../../hessian-matrix.md) is [negative semidefinite](../../../../../../negative-semidefinite-matrix.md), so $0=\Delta u(x_0)\leq\Delta v(x_0)$. At a local minimum the Hessian inequality reverses and gives $\Delta v(x_0)\leq0$. Thus both test conditions hold.

Conversely, suppose only that $u$ is continuous and satisfies the two conditions. We prove the stronger conclusion that these conditions themselves imply $u\in C^\infty$ and $\Delta u=0$. Use the standard Dirichlet existence theorem on a ball: every continuous function on its boundary has a harmonic extension $h\in C^\infty(B_R(a))\cap C(\overline{B_R(a)})$ with exactly those boundary values. This follows, for example, from the Poisson integral. Apply it to $u$ on an arbitrary [relatively compact](../../../../../../relatively-compact-subset.md) ball, obtaining a [harmonic replacement](../../../../../../harmonic-replacement.md) $h$.

If $u-h$ is positive somewhere, choose $\varepsilon>0$ small enough that $u-h-\varepsilon(R^2-|x-a|^2)$ is still positive there. It vanishes on the boundary and therefore has a positive maximum at an interior point. The upper test

$$
v=h+\varepsilon(R^2-|x-a|^2)
$$

has $\Delta v=-2n\varepsilon<0$, contradicting the maximum test condition. Similarly, if $u-h$ is negative somewhere, $v=h-\varepsilon(R^2-|x-a|^2)$ yields an interior negative minimum of $u-v$ for small $\varepsilon$, but $\Delta v=2n\varepsilon>0$, contradicting the minimum condition. Hence $u=h$ throughout the ball.

If the quantifier requires $v\in C^2(\Omega)$ rather than a local test, multiply the displayed smooth $v$ by a smooth cutoff supported within the ball and equal to one near the touching point, extending by zero outside. The resulting global test has the same germ and [Laplacian](../../../../../../laplacian.md) there, so the argument remains valid. Since every point lies in such a ball, $\boxed{u\text{ is a smooth harmonic function throughout }\Omega}$. This is the [continuous viscosity harmonic functions are classical](../../../../../../continuous-viscosity-harmonic-functions-are-classical.md) characterization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
