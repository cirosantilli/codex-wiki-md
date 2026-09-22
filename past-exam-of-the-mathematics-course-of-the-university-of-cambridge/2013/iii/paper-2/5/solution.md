<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $R$ be a [commutative ring](../../../../../commutative-ring.md) and $f=(f_1,\ldots,f_r)$. The [Koszul complex](../../../../../koszul-complex.md) packages these elements and their relations in a finite [chain complex](../../../../../chain-complex.md) of free modules. With $E=R^r$ and basis $e_1,\ldots,e_r$, set $K_i(f;R)=\bigwedge^iE$ for $0\leq i\leq r$, and define

$$
\partial(e_{j_1}\wedge\cdots\wedge e_{j_i})
=\sum_{a=1}^i(-1)^{a-1}f_{j_a}\,
 e_{j_1}\wedge\cdots\wedge\widehat{e_{j_a}}\wedge\cdots\wedge e_{j_i}.
$$

Deleting two distinct basis elements in the two possible orders gives opposite signs and the same coefficient, so $\partial^2=0$. Equivalently $K(f;R)$ is the [tensor product of chain complexes](../../../../../tensor-product-of-chain-complexes.md) of $r$ two-term complexes $[R\xrightarrow{f_i}R]$ in degrees one and zero. The tensor differential is $\partial(u\otimes v)=\partial u\otimes v+(-1)^{\deg u}u\otimes\partial v$. This fixes the sign convention. On the [exterior algebra](../../../../../exterior-algebra.md), the differential is a graded derivation determined by $\partial e_i=f_i$.

For an $R$-[module](../../../../../module-mathematics.md) $M$, define the [Koszul complex with module coefficients](../../../../../koszul-complex-with-module-coefficients.md) by $K(f;M)=K(f;R)\otimes_RM$. Its degree-zero [Koszul homology](../../../../../koszul-homology.md) is

$$
H_0(f;M)=M/(f_1,\ldots,f_r)M.
$$

Its higher [Koszul homology](../../../../../koszul-homology.md) measures the failure of these equations to form a [regular sequence on a module](../../../../../regular-sequence-on-a-module.md). Each $f_j$ annihilates every homology group. Indeed the [Koszul homotopy for multiplication by a generator](../../../../../koszul-homotopy-for-multiplication-by-a-generator.md) is $h_j(u)=e_j\wedge u$, and the graded product rule gives

$$
\partial h_j+h_j\partial=f_j\operatorname{id}.
$$

For coefficients in $M$ the same identity holds after tensoring. Thus multiplication by $f_j$ is zero on homology, and the homology groups are naturally modules over $R/(f)$. If $(f)=R$, choose $\sum_j a_jf_j=1$; then $\sum_j a_jh_j$ is a [contracting homotopy](../../../../../contracting-homotopy.md), so the entire complex is contractible. These identities are also useful after [localization of a ring](../../../../../localization-of-a-ring.md): wherever one generator is a unit, the complex has zero homology.

The construction is functorial under a [ring homomorphism](../../../../../ring-homomorphism.md), and base change gives $K(f;R)\otimes_RS=K(\bar f;S)$, since its terms are free with the displayed basis and differential. An invertible change of generators $f_i=\sum_j u_{ij}g_j$ gives a chain isomorphism by sending $e_i$ to $\sum_j u_{ij}e_j$ and extending to exterior powers. In particular, permuting the generators changes only the exterior signs, not the isomorphism class of the complex.

The essential exactness theorem is that a [regular sequence on a module](../../../../../regular-sequence-on-a-module.md) gives zero positive [Koszul homology](../../../../../koszul-homology.md). Recall that $f_i$ must act injectively on $M/(f_1,\ldots,f_{i-1})M$, with final quotient nonzero. Put $f'=(f_1,\ldots,f_{r-1})$. Adding the final two-term complex identifies $K(f;M)$ with the [mapping cone](../../../../../mapping-cone-homological-algebra.md) of multiplication by $f_r$ on $K(f';M)$, with the chosen tensor signs. The [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) consequently has segments

$$
\cdots\longrightarrow H_i(f';M)\xrightarrow{f_r}H_i(f';M)
\longrightarrow H_i(f;M)\longrightarrow H_{i-1}(f';M)
\xrightarrow{f_r}H_{i-1}(f';M)\longrightarrow\cdots.
$$

For $r=1$, positive homology is exactly $\ker(f_1:M\to M)$. By induction the preceding homology vanishes above zero. The final injectivity assumption kills $H_1(f;M)$, while the exact sequence kills every $H_i$ for $i>1$. Therefore

$$
\boxed{H_i(f;M)=0\ (i>0),\qquad H_0(f;M)=M/(f)M}
$$

for a [regular sequence on a module](../../../../../regular-sequence-on-a-module.md). In particular $K(f;R)$ is a finite [free resolution](../../../../../free-resolution.md) of $R/(f)$ when $f$ is a [regular sequence](../../../../../regular-sequence.md), with ranks $\binom ri$ and length $r$.

There is a precise converse under local finiteness assumptions. Suppose $(R,\mathfrak m)$ is a [Noetherian local ring](../../../../../noetherian-local-ring.md), $0\ne M$ is finitely generated, and all $f_i\in\mathfrak m$. If positive [Koszul homology](../../../../../koszul-homology.md) vanishes, the same exact sequence makes multiplication by $f_r$ surjective on every $H_i(f';M)$ for $i>0$. These modules are finitely generated because the ring is Noetherian and the terms of the complex are finite modules. The [Nakayama lemma](../../../../../nakayama-lemma.md) gives $H_i(f';M)=0$. Induction makes $f'$ regular on $M$, and the degree-one part of the exact sequence makes $f_r$ injective on $H_0(f';M)$. The final quotient is nonzero, again by the [Nakayama lemma](../../../../../nakayama-lemma.md). This proves the [Koszul acyclicity criterion in a Noetherian local ring](../../../../../koszul-acyclicity-criterion-in-a-noetherian-local-ring.md):

$$
\boxed{f\text{ is }M\text{-regular}\iff H_i(f;M)=0\text{ for every }i>0.}
$$

The hypotheses matter: a unit ideal makes the complex contractible but cannot be a proper [regular sequence](../../../../../regular-sequence.md).

Examples make both sides visible. For $R=k[x,y]$ and $f=(x,y)$, the [Koszul resolution](../../../../../koszul-resolution.md) is

$$
0\longrightarrow R\xrightarrow{\binom{-y}{x}}R^2
\xrightarrow{(x\ \ y)}R\longrightarrow k\longrightarrow0.
$$

The signs agree with $\partial(e_1\wedge e_2)=xe_2-ye_1$. For $R=k[x]$ and $f=(x,x)$, the degree-one cycles are $R(1,-1)$ and the boundaries are $xR(1,-1)$; hence $H_1\cong R/(x)$, while $H_2=0$. The repeated element has exposed a relation that the first element already kills.

The [Koszul complex](../../../../../koszul-complex.md) also computes derived functors. If $f$ is a [regular sequence](../../../../../regular-sequence.md) on $R$, its free resolution gives

$$
\operatorname{Tor}_i^R(R/(f),M)=H_i(f;M).
$$

Here no regularity of $f$ on $M$ is assumed. For $S=k[x_1,\ldots,x_r]$, tensor the [Koszul resolution](../../../../../koszul-resolution.md) on the variables with $k$. Every differential becomes zero, so

$$
\operatorname{Tor}_i^S(k,k)\cong\bigwedge^ik^r.
$$

The top group is nonzero, showing that a free resolution of $k$ cannot be shorter than $r$.

Finally, wedging complementary exterior degrees gives a perfect pairing $K_i\otimes_RK_{r-i}\to\bigwedge^rR^r\cong R$. It identifies the dual cochain complex with the degree-reversed [Koszul complex](../../../../../koszul-complex.md), after the appropriate signs. This [self-duality of the Koszul complex](../../../../../self-duality-of-the-koszul-complex.md) shows, for a [regular sequence](../../../../../regular-sequence.md), that

$$
\operatorname{Ext}_R^i(R/(f),R)=0\quad(i\ne r),
\qquad\operatorname{Ext}_R^r(R/(f),R)\cong R/(f).
$$

Thus the same explicit complex simultaneously records quotient equations, regularity, relations, [Tor functor](../../../../../tor-functor.md) computations and [Ext functor](../../../../../ext-functor.md) computations. Its finiteness and exterior structure are what make it especially effective in [commutative algebra](../../../../../commutative-algebra-split.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
