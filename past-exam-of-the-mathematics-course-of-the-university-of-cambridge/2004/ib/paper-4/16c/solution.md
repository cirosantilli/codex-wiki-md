<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

For the [radial Helmholtz Dirichlet Green function](../../../../../radial-helmholtz-dirichlet-green-function.md), set $H(x,\xi)=xG(x,\xi)$. Multiplication of the radial equation by $x$ gives

$$
H_{xx}+k^2H=\xi\delta(x-\xi),\qquad H(0,\xi)=H(1,\xi)=0.
$$

The first endpoint follows from the required boundedness of $G$ at zero. For $k\ne0$ and $\sin k\ne0$, use the left solution $\sin kx$ and right solution $\sin k(1-x)$. Their [Wronskian](../../../../../wronskian.md) is $-k\sin k$. Matching continuity and the derivative jump therefore gives, with $x_< =\min(x,\xi)$ and $x_> =\max(x,\xi)$,

$$
\boxed{G(x,\xi)=-\frac{\xi\sin(kx_<)\sin(k(1-x_>))}{kx\sin k}.}
$$

This is finite at zero, vanishes at one, is continuous at $x=\xi$, and has $G_x(\xi+,\xi)-G_x(\xi-,\xi)=1$. Thus it has exactly the prescribed delta source, not its negative. Its weighted reciprocity is $x^2G(x,\xi)=\xi^2G(\xi,x)$, as expected for the radial weight.

Integrating the [Green function](../../../../../green-s-function.md) against the constant forcing gives

$$
y(x)=-\frac1{kx\sin k}\left[\sin(k(1-x))\int_0^x\xi\sin(k\xi)d\xi+\sin(kx)\int_x^1\xi\sin(k(1-\xi))d\xi\right].
$$

The integrals are respectively $-x\cos(kx)/k+\sin(kx)/k^2$ and $(1-x\cos(k(1-x)))/k-\sin(k(1-x))/k^2$. After cancellation their weighted sum is $(\sin(kx)-x\sin k)/k$. Hence

$$
\boxed{y(x)=\frac1{k^2}\left(1-\frac{\sin(kx)}{x\sin k}\right).}
$$

The values at zero are interpreted by continuity. At $k=0$ the limit exists: $G(x,\xi)=-\xi x_<(1-x_>)/x$ and **$y(x)=(x^2-1)/6$**.

The exceptional nonzero values $k\in\pi\mathbb Z$ need a genuine qualification. There is then a nonzero bounded homogeneous solution $\sin(kx)/x$ satisfying both endpoint conditions, so an inverse Green function does not exist. Moreover the stated forcing is incompatible, not merely nonunique. If $h=xy$ solved the problem, multiply $h''+k^2h=x$ by $\sin(kx)$ and integrate by parts using $h(0)=h(1)=0$. The left side is zero, whereas

$$
\int_0^1x\sin(kx)dx=-\frac{\cos k}{k}\ne0.
$$

Thus **there is no solution for nonzero $k\in\pi\mathbb Z$**. This explains exactly when the generic formula is applicable.

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
