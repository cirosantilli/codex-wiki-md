<h1 id="11d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Away from the source point, the [Green function](../../../../../../green-s-function.md) obeys the homogeneous equation and must satisfy the appropriate endpoint condition. Thus it has the form $A\sin(kx)$ to the left of $\xi$ and $B\sin(k(\pi-x))$ to the right. It must be continuous at $\xi$: otherwise its second distributional derivative would contain an unwanted derivative of a [Dirac delta](../../../../../../dirac-delta-function.md). Integrating across $\xi$ gives the jump condition $G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=1$.

The left and right homogeneous solutions $u=\sin(kx)$, $v=\sin(k(\pi-x))$ have constant [Wronskian](../../../../../../wronskian.md)

$$
uv'-u'v=-k\sin(k\pi).
$$

This is nonzero for real noninteger $k$. Dividing the product of the left and right solutions by that Wronskian therefore gives the [Dirichlet Helmholtz Green function on an interval](../../../../../../dirichlet-helmholtz-green-function-on-an-interval.md)

$$
\boxed{G(x,\xi)=-\frac{\sin(k\min(x,\xi))\sin(k(\pi-\max(x,\xi)))}{k\sin(k\pi)}.}
$$

The formula vanishes at both endpoints, is continuous at the source and has derivative jump one, verifying all distributional and boundary conditions. A difference of two such Green functions would be a homogeneous Dirichlet solution; it vanishes because $\sin(k\pi)\ne0$, proving uniqueness. Although zero is excluded by the stated noninteger condition, the removable $k\to0$ limit is $-\min(x,\xi)(\pi-\max(x,\xi))/\pi$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
