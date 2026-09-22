<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set

$$
A(t)=\int_0^t a(s)\,ds.
$$

The [scalar conservation law](../../../../../../scalar-conservation-law.md) is $u_t+a(t)f'(u)u_x=0$. Its [characteristic curve](../../../../../../characteristic-curve.md) issuing from $\xi$ satisfies

$$
X(t;\xi)=\xi+A(t)f'(u_0(\xi)),
\qquad
u(t,X(t;\xi))=u_0(\xi).
$$

The [Jacobian](../../../../../../jacobian-matrix.md) of the one-dimensional characteristic map is

$$
X_\xi(t;\xi)=1+A(t)m(\xi),
\qquad
m(\xi)=f''(u_0(\xi))u_0'(\xi).
$$

Before [characteristic crossing](../../../../../../characteristic-crossing.md), differentiation with respect to $\xi$ gives

$$
u_x(t,X(t;\xi))
=\frac{u_0'(\xi)}{1+A(t)m(\xi)}.
$$

Because $u_0$ has [compact support](../../../../../../compact-support.md), $m$ is continuous and vanishes outside a compact set. It therefore attains its minimum

$$
m_*=\min_{\xi\in\mathbb R}m(\xi)<0
$$

by the hypothesis. Since $a(t)>\varepsilon$, the function $A$ is strictly increasing and tends to infinity. There is consequently a unique first time $T_*>0$ satisfying

$$
\int_0^{T_*}a(s)\,ds=A(T_*)=-\frac1{m_*}.
$$

At a minimizer of $m$, the numerator $u_0'$ is nonzero because $f''$ is nonzero, while the denominator tends to zero as $t\uparrow T_*$. Hence the classical solution has [gradient blow-up](../../../../../../gradient-blow-up.md):

$$
\boxed{\lVert u_x(t,\cdot)\rVert_{L^\infty(\mathbb R)}\longrightarrow\infty
\qquad(t\uparrow T_*).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
