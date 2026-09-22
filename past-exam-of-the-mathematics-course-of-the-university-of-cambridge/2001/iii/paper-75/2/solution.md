<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Normalize the weight-four and weight-six [Eisenstein series](../../../../../eisenstein-series.md) to have constant term one. Their [Fourier expansions](../../../../../fourier-series-split.md) begin

$$
E_4=1+240q+O(q^2),\qquad E_6=1-504q+O(q^2),\qquad q=e^{2\pi iz}.
$$

Their absolutely convergent lattice sums transform by [modular weights](../../../../../weight-of-a-modular-form.md) four and six under reindexing by the [modular group](../../../../../modular-group.md), and their [Fourier expansions](../../../../../fourier-series-split.md) prove holomorphy at its [modular cusp](../../../../../cusp-of-a-modular-group.md). Thus they are elements of $M_4,M_6$.

We use the [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md): for a nonzero weight-$k$ form,

$$
v_\infty(f)+\tfrac12v_i(f)+\tfrac13v_\rho(f)+\sum_{z\ne i,\rho}v_z(f)=\frac{k}{12}.
$$

The sum uses one point of each ordinary orbit. This is the argument principle on a truncated fundamental region: paired vertical integrals cancel, the circle pairing $f(-1/z)=z^kf(z)$ contributes the [modular weight](../../../../../weight-of-a-modular-form.md) term, and local quotient coordinates at the two [elliptic points of a modular curve](../../../../../elliptic-point-of-a-modular-curve.md) [modular weight](../../../../../weight-of-a-modular-form.md) their orders by $1/2,1/3$. All orders are nonnegative for a holomorphic [modular form](../../../../../modular-form.md).

Define the [modular discriminant](../../../../../modular-discriminant.md) by

$$
\Delta=\frac{E_4^3-E_6^2}{1728}=q+O(q^2).
$$

It is a weight-twelve [cusp form](../../../../../cusp-form.md). Its order at infinity is one, exhausting the valence total $12/12=1$. Hence $\Delta$ has no zeros in $\mathbb H$. Therefore every weight-$k$ [cusp form](../../../../../cusp-form.md) is divisible by $\Delta$, with quotient holomorphic on $\mathbb H$ and at the [modular cusp](../../../../../cusp-of-a-modular-group.md):

$$
\boxed{S_k=\Delta M_{k-12}.}
$$

Negative [modular weights](../../../../../weight-of-a-modular-form.md) vanish by the valence formula, and odd [modular weights](../../../../../weight-of-a-modular-form.md) vanish because $-I$ acts by $(-1)^k$. Weight-zero forms are constant: they descend holomorphically to the [compactified modular curve](../../../../../compactified-modular-curve.md), and the [maximum modulus principle](../../../../../maximum-modulus-principle.md) applies. There are no weight-two forms: $f(i)=i^2f(i)=-f(i)$ forces a zero at $i$, whose valence contribution $1/2$ exceeds $2/12$.

Every nonnegative even [modular weight](../../../../../weight-of-a-modular-form.md) other than two is $4a+6b$ with $a,b\geq0$. If $k\equiv0\pmod4$, take $b=0$; if $k\equiv2\pmod4$ and $k\geq6$, take $b=1$. For $f\in M_k$, choose such a monomial $h=E_4^aE_6^b$, whose constant term is one. Subtracting the constant term $c$ of $f$ gives $f-ch\in S_k$, so

$$
f=cE_4^aE_6^b+\Delta g,\qquad g\in M_{k-12}.
$$

Induction on [modular weight](../../../../../weight-of-a-modular-form.md), together with $1728\Delta=E_4^3-E_6^2$, proves that every [modular form](../../../../../modular-form.md) is a [polynomial](../../../../../polynomial-split.md) in $E_4,E_6$.

For [algebraic independence](../../../../../algebraic-independence.md), first fix one [modular weight](../../../../../weight-of-a-modular-form.md) $w$. All solutions of $4a+6b=w$ have the same residue of $a$ modulo three and the same parity of $b$. Consequently their monomials can be written

$$
E_4^{a_0}E_6^{b_0}(E_4^3)^j(E_6^2)^{L-j},\qquad j=0,\ldots,L,
$$

for suitable $a_0,b_0,L$. On an open set where the common factor and $E_6$ are nonzero, a linear relation would give a [polynomial](../../../../../polynomial-split.md) relation in

$$
R(z)=\frac{E_4(z)^3}{E_6(z)^2}=1+1728q+O(q^2).
$$

This is nonconstant. By the [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md), a [polynomial](../../../../../polynomial-split.md) vanishing on all its values must be the zero [polynomial](../../../../../polynomial-split.md). Thus same-weight monomials are linearly independent.

Different [modular weights](../../../../../weight-of-a-modular-form.md) cannot cancel either. Suppose $\sum_w P_w(E_4,E_6)=0$ with each $P_w$ weighted homogeneous. Transform by $\gamma_n=\begin{pmatrix}1&0\\n&1\end{pmatrix}$. At any fixed $z\in\mathbb H$ this gives

$$
\sum_w(nz+1)^wP_w(E_4(z),E_6(z))=0\qquad(n\in\mathbb Z).
$$

The numbers $nz+1$ are infinitely many distinct values, so the [polynomial](../../../../../polynomial-split.md) in that number vanishes identically, and every $P_w(z)=0$. The same-weight independence then sets every [coefficient](../../../../../coefficient.md) to zero. This is the [graded weights separate analytic polynomial relations](../../../../../graded-weights-separate-analytic-polynomial-relations.md) argument. Hence

$$
\boxed{M_*(SL_2(\mathbb Z))\cong\mathbb C[E_4,E_6],\qquad \deg E_4=4,\ \deg E_6=6,}
$$

with **algebraically independent generators**. Multiplying the two [Eisenstein series](../../../../../eisenstein-series.md) by their nonzero lattice-normalization constants does not alter either generation or independence.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
