<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Let $V_n$ be the space of homogeneous degree-$n$ polynomials in $x,y$. For $g\in SU(2)$ and a column vector $v=(x,y)^T$, define

$$
(\rho_n(g)P)(v)=P(g^{-1}v).
$$

Substitution preserves degree, and

$$
\rho_n(gh)P(v)=P(h^{-1}g^{-1}v)
=\rho_n(g)\rho_n(h)P(v),
$$

so $\rho_n:SU(2)\to\operatorname{GL}(V_n)$ is a [continuous representation of a topological group](../../../../../continuous-representation-of-a-topological-group.md). This is the [homogeneous polynomial representation of SU2](../../../../../homogeneous-polynomial-representation-of-su2.md).

To prove [irreducibility](../../../../../irreducible-representation.md), restrict to the diagonal circle

$$
t_\theta=\operatorname{diag}(e^{i\theta},e^{-i\theta}).
$$

The monomials $x^{n-k}y^k$ are its one-dimensional weight spaces, with distinct weights up to our harmless inverse-action convention. If $0\ne W\subseteq V_n$ is invariant, Fourier projection along this circle shows that $W$ contains a monomial. Differentiating the action of $SU(2)$ and complexifying gives the operators

$$
E=x\frac{\partial}{\partial y},
\qquad
F=y\frac{\partial}{\partial x}.
$$

Repeated applications of $E$ and $F$ connect every monomial $x^{n-k}y^k$ to every other one. Hence $W$ contains the entire monomial basis, so $W=V_n$.

Every $g\in SU(2)$ is conjugate to $\operatorname{diag}(z,z^{-1})$ with $|z|=1$. Reading the eigenvalues on the monomial basis gives the [character of the homogeneous polynomial representation of SU2](../../../../../character-of-the-homogeneous-polynomial-representation-of-su2.md)

$$
\boxed{
\chi_n(g)=z^n+z^{n-2}+\cdots+z^{-n}
}.
$$

For $z=e^{i\theta}$ this is

$$
\chi_n(g)=\frac{\sin((n+1)\theta)}{\sin\theta},
$$

with the values at $\sin\theta=0$ obtained by continuity.

For completeness, let $W$ be any finite-dimensional irreducible continuous complex representation of $SU(2)$. Its restriction to the diagonal circle splits into integral weight spaces. Choose a vector of largest weight $n$. The raising operator kills it, and the $\mathfrak{sl}_2$ commutation relations show that $n$ is a nonnegative integer and that successive applications of the lowering operator form a string of weights

$$
n,n-2,\ldots,-n.
$$

Their span is an invariant copy of $V_n$; irreducibility forces it to equal $W$. Thus the [classification of finite-dimensional representations of SU2](../../../../../classification-of-finite-dimensional-representations-of-su2.md) says

$$
\boxed{W\cong V_n\quad\text{for a unique }n\geq0}.
$$

If the eigenvalues of $\rho(g)$ are $\lambda_1,\ldots,\lambda_d$, then the eigenvalues on $\bigwedge^2V$ are $\lambda_i\lambda_j$ for $i<j$. Therefore the [character of an exterior square](../../../../../character-of-an-exterior-square.md) is

$$
\boxed{
\chi_{\wedge^2V}(g)
=\frac12\bigl(\chi(g)^2-\chi(g^2)\bigr)
}.
$$

The [exterior square of an SU2 irreducible representation](../../../../../exterior-square-of-an-su2-irreducible-representation.md) or the [Clebsch-Gordan decomposition for SU2](../../../../../clebsch-gordan-decomposition-for-su2.md) with flip parity gives

$$
\boxed{\bigwedge^2V_4\cong V_6\oplus V_2}.
$$

The dimensions $7+3=10=\binom52$ check the result.

The third [elementary symmetric polynomial](../../../../../elementary-symmetric-polynomial.md) in the $\lambda_i$, together with [Newton identities](../../../../../newton-s-identities.md), gives

$$
\boxed{
\chi_{\wedge^3V}(g)
=\frac16\left(
\chi(g)^3-3\chi(g)\chi(g^2)+2\chi(g^3)
\right)
}.
$$

For the five-dimensional representation $V_4$, the canonical duality

$$
\bigwedge^3V_4
\cong(\bigwedge^2V_4)^*\otimes\det V_4
$$

finishes the decomposition. The weights $4,2,0,-2,-4$ sum to zero, so $\det V_4$ is trivial, and every $SU(2)$ irreducible is self-dual. Consequently

$$
\boxed{\bigwedge^3V_4\cong V_6\oplus V_2}.
$$

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
