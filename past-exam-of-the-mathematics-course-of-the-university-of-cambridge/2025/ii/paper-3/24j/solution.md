<h1 id="24j/solution">Solution</h1>

↑ **Parent:** [24J](../24j.md)

Let

$$
A_V=k[x_0,\ldots,x_n]/I(V)
$$

be the homogeneous coordinate ring. Its Hilbert function agrees for all sufficiently large $m$ with a polynomial $P_V(m)$. Since $V$ is a curve,

$$
P_V(m)=dm+c.
$$

The [degree of a projective curve](../../../../../degree-of-a-projective-curve.md) is the positive integer $d$. This is well-defined because the graded ring $A_V$, and hence its eventual [Hilbert polynomial](../../../../../hilbert-polynomial.md), depends only on the embedded projective variety, while a polynomial agreeing with the Hilbert function for all large integers is unique.

This definition also has the geometric interpretation expected of degree. For a sufficiently general hyperplane $H=Z(\ell)$ that does not contain $V$, multiplication by $\ell$ gives an exact sequence

$$
0\longrightarrow A_V(-1)
\xrightarrow{\ \ell\ }A_V
\longrightarrow A_V/(\ell)\longrightarrow0.
$$

Consequently, for large $m$,

$$
\dim_k(A_V/(\ell))_m
=P_V(m)-P_V(m-1)=d.
$$

The left side is the length of the zero-dimensional scheme $V\cap H$. Thus a generic hyperplane meets $V$ in $d$ points counted with intersection multiplicity, independently of the chosen generic hyperplane.

For the stated linear embedding, the homogeneous coordinate ring of $\varphi(V)$ is

$$
\frac{k[x_0,\ldots,x_m]}
{I(V)+(x_{n+1},\ldots,x_m)}
\cong
\frac{k[x_0,\ldots,x_n]}{I(V)}.
$$

The graded rings have the same Hilbert polynomial, so [degree under a linear projective embedding](../../../../../degree-under-a-linear-projective-embedding.md) gives

$$
\deg_{\mathbb P^m}\varphi(V)=\deg_{\mathbb P^n}V.
$$

Degree is nevertheless not an invariant of an abstract curve. In $\mathbb P^2$, a line has degree one and the smooth conic

$$
x_0x_2-x_1^2=0
$$

has degree two, but the map

$$
[s:t]\longmapsto[s^2:st:t^2]
$$

identifies the conic with $\mathbb P^1$, as is any projective line.

For the specified set $S$, the equations are the $2\times2$ minors of

$$
\begin{pmatrix}
x_0&x_1&x_2\\
x_1&x_2&x_3
\end{pmatrix}.
$$

On the affine chart $x_0=1$, they force

$$
x_2=x_1^2,\qquad x_3=x_1^3,
$$

so this chart is an affine line. When $x_0=0$, the equations force $x_1=x_2=0$, leaving the single point $[0:0:0:1]$. Hence $V$ is the [twisted cubic](../../../../../twisted-cubic.md), parametrized by

$$
[s:t]\longmapsto[s^3:s^2t:st^2:t^3].
$$

It is therefore an irreducible projective curve. A generic hyperplane pulls back to a binary cubic

$$
a_0s^3+a_1s^2t+a_2st^2+a_3t^3,
$$

which has three zeros on $\mathbb P^1$ counted with multiplicity. Thus

$$
\boxed{\deg V=3}.
$$

No nonzero linear form vanishes on $V$, since substituting its parametrization would make the four coefficients of the displayed binary cubic vanish. Therefore every hypersurface containing $V$ has degree at least two. If

$$
V=Z(F_1,\ldots,F_r),
$$

then $r=1$ is impossible because a nonzero hypersurface in $\mathbb P^3$ has dimension two. Hence at least two nonconstant $F_i$ are needed, and

$$
\prod_i\deg Z(F_i)\geq2\cdot2=4>3=\deg V.
$$

This is the [degree obstruction to the twisted cubic being a complete intersection](../../../../../degree-obstruction-to-the-twisted-cubic-being-a-complete-intersection.md).

Finally compare the twisted cubic with a smooth plane cubic, such as

$$
E=Z(x_0^3+x_1^3+x_2^3)\subset\mathbb P^2,
$$

viewed in $\mathbb P^3$ by the given linear embedding. Both curves are irreducible and have degree three. The twisted cubic is isomorphic to $\mathbb P^1$ and has genus zero, whereas the supplied plane-curve genus formula gives

$$
g(E)=\frac{(3-1)(3-2)}2=1.
$$

Since genus is an isomorphism invariant, these equal-degree curves are not isomorphic.

## ↑ Ancestors (10)

1. [24J](../24j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
