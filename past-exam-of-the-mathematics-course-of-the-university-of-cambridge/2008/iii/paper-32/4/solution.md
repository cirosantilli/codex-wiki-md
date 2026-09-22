<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Realize the two-dimensional [irreducible representation](../../../../../irreducible-representation.md) $\rho$ as the [standard representation of the symmetric group](../../../../../standard-representation-of-the-symmetric-group.md) on

$$
V=\{(z_1,z_2,z_3)\in\mathbb C^3:z_1+z_2+z_3=0\},
$$

with $S_3$ permuting coordinates. It is the complement of the trivial summand in the three-point [permutation representation](../../../../../permutation-representation.md). For each prime the [local factor of an Artin L-function](../../../../../local-factor-of-an-artin-l-function.md) is

$$
L_p(\rho,s)=\det\bigl(1-p^{-s}\rho(\operatorname{Frob}_p)\vert_{V^{I_p}}\bigr)^{-1},
$$

where $I_p$ is the [inertia group](../../../../../inertia-group.md) and Frobenius means any lift of the residue-field [Frobenius automorphism](../../../../../frobenius-automorphism.md). On $V^{I_p}$ the lift is independent of that choice. At an unramified prime, put $t=p^{-s}$. The [Local Artin factors of the standard representation of S3](../../../../../local-artin-factors-of-the-standard-representation-of-s3.md) are

$$
\begin{array}{c|c|c}
\text{Frobenius cycle type}&\text{eigenvalues on }V&L_p(\rho,s)\\\hline
(1)(2)(3)&1,1&(1-t)^{-2}\\
(12)&1,-1&(1-t^2)^{-1}\\
(123)&\zeta_3,\zeta_3^2&(1+t+t^2)^{-1}.
\end{array}
$$

The [polynomial discriminant](../../../../../polynomial-discriminant.md) of $X^3-3$ is $-243=-3^5$, so only $3$ can ramify in its [splitting field](../../../../../splitting-field.md). For $p\ne3$, the squarefree factorization of $X^3-3$ modulo $p$ determines the [Frobenius cycle type](../../../../../frobenius-cycle-type.md) on its roots.

At $p=2$,

$$
X^3-3\equiv(X+1)(X^2+X+1)\pmod2.
$$

The quadratic is irreducible, so Frobenius is a transposition and

$$
L_2(\rho,s)=\frac1{1-2^{-2s}}=1+2^{-2s}+2^{-4s}+\cdots.
$$

Thus $a_2=0$, $a_4=1$ and $a_8=0$. At $p=5$,

$$
X^3-3\equiv(X-2)(X^2+2X+4)\pmod5.
$$

The quadratic discriminant is $3\pmod5$, a nonsquare, so this is again a transposition. Consequently $L_5(\rho,s)=(1-5^{-2s})^{-1}$ and $a_5=0$.

At $p=7$, the possible cubes are $0,1,-1$, so $X^3-3$ has no root modulo $7$. Being cubic, it is irreducible; Frobenius is a three-cycle. Therefore

$$
L_7(\rho,s)=\frac1{1+7^{-s}+7^{-2s}}=\frac{1-7^{-s}}{1-7^{-3s}}=1-7^{-s}+O(7^{-3s}),
$$

and $a_7=-1$.

The ramified factor at $3$ must be computed on [inertia group](../../../../../inertia-group.md) invariants. Write $\alpha=3^{1/3}$ and set $\pi=(\zeta_3-1)/\alpha$. Using $(\zeta_3-1)^2=-3\zeta_3$ gives

$$
\pi^3=1+2\zeta_3,\qquad\pi^6=-3.
$$

The [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) $X^6+3$ over $\mathbb Q_3$ has degree six, so $\mathbb Q_3(\pi)$ is a totally ramified degree-six subfield of $\mathbb Q_3(\zeta_3,\alpha)$. The latter has degree at most $[F:\mathbb Q]=6$, so the fields agree. This [Eisenstein sextic presentation of the splitting field of X3 minus 3 over Q3](../../../../../eisenstein-sextic-presentation-of-the-splitting-field-of-x3-minus-3-over-q3.md) shows $D_3=I_3=S_3$. Since the only permutation-invariant vectors in $\mathbb C^3$ have all coordinates equal, their intersection with $V$ is zero. Thus

$$
\boxed{V^{I_3}=0,\qquad L_3(\rho,s)=1.}
$$

In particular $a_3=a_9=0$; an unramified degree-two factor at $3$ would give the wrong coefficients.

Finally the [Euler product](../../../../../euler-product.md) makes its [Dirichlet series](../../../../../dirichlet-series.md) coefficients multiplicative for coprime indices. Its constant coefficient is $a_1=1$, and $a_6=a_2a_3=0$, $a_{10}=a_2a_5=0$. Every integer up to ten is now covered, giving

$$
\boxed{(a_1,a_2,a_3,a_4,a_5,a_6,a_7,a_8,a_9,a_{10})=(1,0,0,1,0,0,-1,0,0,0).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
