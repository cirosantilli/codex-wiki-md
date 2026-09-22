<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For radial data, set

$$
f_0(r)=r\,u_0(|r|),\qquad f_1(r)=r\,u_1(|r|)
$$

on $\mathbb R$. The conditions at the origin say exactly that these are smooth odd compactly supported functions. The radial reduction $w(t,r)=ru(t,r)$ satisfies the one-dimensional wave equation, and the [D'Alembert formula](../../../../../../d-alembert-s-formula.md) gives

$$
w(t,r)=\frac12\big(f_0(r-t)+f_0(r+t)\big)
+\frac12\int_{r-t}^{r+t}f_1(s)\,ds.
$$

In null coordinates this is

$$
w=\frac12\big(f_0(-\xi)+f_0(\eta)\big)
+\frac12\int_{-\xi}^{\eta}f_1(s)\,ds.
$$

The limits are therefore

$$
\psi_+(\xi)=
\frac12f_0(-\xi)+\frac12\int_{-\xi}^{\infty}f_1(s)\,ds,
$$



$$
\psi_-(\eta)=
\frac12f_0(\eta)-\frac12\int_{\eta}^{\infty}f_1(s)\,ds.
$$

They are smooth and compactly supported because $f_0,f_1$ are odd.

Write

$$
A(s)=\frac12f_0(s),\qquad
B(s)=\frac12\int_s^\infty f_1(q)\,dq.
$$

Then $A$ is an arbitrary odd test function and $B$ is an arbitrary even test function. Conversely, every odd $A\in C_c^\infty(\mathbb R)$ gives $f_0=2A$, and every even $B\in C_c^\infty(\mathbb R)$ gives $f_1=-2B'$. Thus both maps are injective and

$$
X_-=X_+=C_c^\infty(\mathbb R).
$$

Since

$$
\psi_-=A-B,\qquad
\psi_+=-A+B,
$$

the radial [scattering map](../../../../../../scattering-map.md) is

$$
\boxed{S\psi=-\psi.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
