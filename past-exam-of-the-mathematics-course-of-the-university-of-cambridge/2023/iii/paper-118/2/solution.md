<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [irreducible complex analytic hypersurface](../../../../../complex-analytic-hypersurface.md) in a [complex manifold](../../../../../complex-manifold.md) $X$ is a closed irreducible analytic subset of pure complex codimension one. A [local defining function of a complex analytic hypersurface](../../../../../local-defining-function-of-a-complex-analytic-hypersurface.md) $Y$ at $x$ is a holomorphic function $f$ on a neighbourhood $U$ such that

$$
Y\cap U=\{f=0\}.
$$

The necessary local algebra is that the stalk $\mathcal O_{X,x}$ is a [regular local ring](../../../../../regular-local-ring.md), hence a [unique factorization domain](../../../../../unique-factorization-domain.md), and that the local branches of a hypersurface germ determine finitely many height-one [prime ideals](../../../../../prime-ideal.md). Each is principal; the product of their generators gives $f$, and removing repeated factors makes it reduced. This also covers a globally irreducible hypersurface that has several local branches at a singular point.

A [divisor on a complex manifold](../../../../../divisor-on-a-complex-manifold.md) is a locally finite formal sum $D=\sum_Yn_YY$ of irreducible analytic hypersurfaces with integer coefficients. On a sufficiently small $U_\alpha$, local defining functions give a meromorphic equation $f_\alpha$ for $D$. The quotients $f_\alpha/f_\beta$ are nowhere-zero holomorphic functions. Gluing frames by

$$
e_\alpha=(f_\beta/f_\alpha)e_\beta
$$

produces the [holomorphic line bundle associated to a divisor](../../../../../holomorphic-line-bundle-associated-to-a-divisor.md) $[D]$, and $f_\alpha e_\alpha$ gives its canonical meromorphic section with divisor $D$.

The [Euler sequence on complex projective space](../../../../../euler-sequence-on-complex-projective-space.md)

$$
0\longrightarrow\mathcal O
\longrightarrow\mathcal O(1)^{\oplus(n+1)}
\longrightarrow T\mathbb{CP}^n
\longrightarrow0
$$

implies $\det T\mathbb{CP}^n\cong\mathcal O(n+1)$. Taking the dual determinant yields the [canonical bundle of complex projective space](../../../../../canonical-bundle-of-complex-projective-space.md)

$$
K_{\mathbb{CP}^n}\cong\mathcal O(-n-1)\cong[-(n+1)H],
$$

where $H$ is a [hyperplane divisor](../../../../../hyperplane-divisor.md).

The hypotheses on the homogeneous polynomial $p$ say that

$$
V=\{p=0\}\subset\mathbb{CP}^n
$$

is a smooth [projective hypersurface](../../../../../projective-hypersurface.md) of degree $k$, so its divisor line bundle is $[V]\cong\mathcal O(kH)$. The [adjunction formula](../../../../../adjunction-formula.md) gives

$$
K_V
\cong\bigl(K_{\mathbb{CP}^n}\otimes[V]\bigr)|_V
\cong\mathcal O_V(k-n-1)
\cong[(k-n-1)H|_V].
$$

This is the [canonical bundle of a smooth projective hypersurface](../../../../../canonical-bundle-of-a-smooth-projective-hypersurface.md).

Now fix an isomorphism $\Phi:[P]\to[Q]$ and regard $s_P$ and $\Phi^{-1}s_Q$ as [holomorphic sections](../../../../../holomorphic-section.md) of the same [holomorphic line bundle](../../../../../holomorphic-line-bundle.md). They have no common zero because $P\ne Q$. Their homogeneous coordinates therefore define a well-defined [holomorphic map](../../../../../holomorphic-map.md)

$$
F:S\longrightarrow\mathbb{CP}^1,
\qquad
F(x)=[s_P(x):\Phi^{-1}s_Q(x)].
$$

In a local frame, the quotient

$$
f=\frac{s_P}{\Phi^{-1}s_Q}
$$

is a [meromorphic function](../../../../../meromorphic-function.md) with divisor $(f)=P-Q$. Thus $F^{-1}(0)=P$ and $F^{-1}(\infty)=Q$, both with multiplicity one. The [degree of a holomorphic map](../../../../../degree-of-a-holomorphic-map.md) $F$ is therefore one. A nonconstant degree-one holomorphic map between compact connected [Riemann surfaces](../../../../../riemann-surfaces.md) is a [biholomorphism](../../../../../biholomorphism.md), so the displayed map is biholomorphic.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
