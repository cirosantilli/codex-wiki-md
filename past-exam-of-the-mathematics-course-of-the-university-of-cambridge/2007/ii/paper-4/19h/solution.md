<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

We consider finite-dimensional continuous complex representations of [SU(2)](../../../../../su-2-group.md). Its maximal [torus](../../../../../torus.md) is $\operatorname{diag}(e^{i\theta},e^{-i\theta})$. The [irreducible representations](../../../../../irreducible-representation.md) are

$$
\boxed{V_n=\operatorname{Sym}^n(\mathbb C^2),\qquad n=0,1,2,\ldots,\qquad \dim V_n=n+1.}
$$

They may be realized as homogeneous [polynomials](../../../../../polynomial-split.md) of degree $n$ in two variables, with the induced linear substitution action. Their [torus](../../../../../torus.md) weights are $n,n-2,\ldots,-n$, each once. The centre $-I$ acts by $(-1)^n$, so precisely the even-$n$ representations descend to [SO(3)](../../../../../so-3-group.md). In physics $n=2j$ labels integral or half-integral spin $j$.

Here is a classification argument. Average any positive definite Hermitian form over the compact group using normalized [Haar measure](../../../../../haar-measure.md). The averaged form is invariant, so the orthogonal complement of an [invariant subspace](../../../../../invariant-subspace.md) is invariant. Repeatedly splitting gives complete reducibility. Differentiate an [irreducible representation](../../../../../irreducible-representation.md) and complexify to the [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak{sl}_2$, with generators $H,E,F$ satisfying $[H,E]=2E$, $[H,F]=-2F$, and $[E,F]=H$. [Torus](../../../../../torus.md) periodicity gives integer $H$-weights. Choose a vector $v$ of maximal weight $n$; then $Ev=0$. Induction on $k$ using the commutators gives

$$
EF^kv=k(n-k+1)F^{k-1}v.
$$

The chain terminates: if $F^{p}v\ne0$ and $F^{p+1}v=0$, the displayed formula forces $n=p\geq0$. The vectors $v,Fv,\ldots,F^nv$ have distinct weights, span an invariant subrepresentation, and hence span the [irreducible representation](../../../../../irreducible-representation.md). Their generator action agrees with $\operatorname{Sym}^n\mathbb C^2$. Invariance under the [Lie algebra](../../../../../lie-algebra-split.md) is equivalent to invariance under the connected group, completing the classification. Conversely, a nonzero [invariant subspace](../../../../../invariant-subspace.md) of a [symmetric power](../../../../../symmetric-power.md) contains a weight vector by projection onto [torus](../../../../../torus.md) weights. Raising it to the [highest weight](../../../../../highest-weight-of-a-representation.md) and then lowering generates every monomial, proving that the [symmetric power](../../../../../symmetric-power.md) is irreducible.

The character on the [torus](../../../../../torus.md) is

$$
\chi_n(\theta)=\sum_{k=0}^n e^{i(n-2k)\theta}
=\frac{\sin((n+1)\theta)}{\sin\theta},
$$

with the endpoints interpreted by continuity. Every representation has a unique decomposition $V\cong\bigoplus_{n\geq0}m_nV_n$. Its multiplicities can be computed from character inner products,

$$
\boxed{m_n=\int_{\mathrm{SU}(2)}\chi_V(g)\overline{\chi_n(g)}\,dg
=\frac2\pi\int_0^\pi\chi_V(\theta)\chi_n(\theta)\sin^2\theta\,d\theta.}
$$

The sine orthogonality directly verifies orthonormality of the irreducible characters. Alternatively, if $w_k$ is the dimension of the weight-$k$ subspace, the weight lists give $w_n=m_n+m_{n+2}+\cdots$, so **$m_n=w_n-w_{n+2}$** for $n\geq0$. This gives a constructive decomposition from [torus](../../../../../torus.md) weights. In particular, multiplying weight characters yields the [Clebsch-Gordan decomposition](../../../../../clebsch-gordan-decomposition.md) $V_m\otimes V_n\cong V_{m+n}\oplus V_{m+n-2}\oplus\cdots\oplus V_{|m-n|}$. Arbitrary unitary Hilbert-space representations of this compact group similarly decompose into Hilbert [direct sums](../../../../../direct-sum.md) of these finite-dimensional irreducibles; the finite-dimensional statement above is the standard representation-theory setting.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
