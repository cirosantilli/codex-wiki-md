<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a finite-rank [free abelian group](../../../../../../free-abelian-group.md) $H_{\mathbb Z}$. A pure integral [Hodge structure](../../../../../../hodge-structure.md) of weight $w$ is a decomposition

$$
H_{\mathbb C}=H_{\mathbb Z}\otimes\mathbb C
=\bigoplus_{p+q=w}H^{p,q},
\qquad \overline{H^{p,q}}=H^{q,p}.
$$

Its [Hodge numbers](../../../../../../hodge-number.md) are $h^{p,q}=\dim_{\mathbb C}H^{p,q}$, and its [Hodge filtration](../../../../../../hodge-filtration.md) is $F^p=\bigoplus_{r\ge p}H^{r,w-r}$. Equivalently, the filtration has these dimensions and satisfies

$$
H_{\mathbb C}=F^p\oplus\overline{F^{w-p+1}}.
$$

The decomposition is recovered as $H^{p,q}=F^p\cap\overline{F^q}$.

A [polarized Hodge structure](../../../../../../polarized-hodge-structure.md) additionally has a nondegenerate integral [bilinear form](../../../../../../bilinear-form.md) $Q$ satisfying $Q(u,v)=(-1)^wQ(v,u)$, extended complex-bilinearly, with

$$
Q(H^{p,q},H^{r,s})=0\quad\text{unless }(r,s)=(q,p).
$$

We choose the geometric sign convention in which the positivity condition is

$$
\boxed{(-1)^{w(w-1)/2}i^{p-q}Q(v,\bar v)>0
\quad(0\ne v\in H^{p,q}).}
$$

The expression is real by the symmetry and conjugation conditions. In particular it is $iQ(v,\bar v)>0$ on a weight-one $(1,0)$ summand. Other conventions absorb the constant factor $(-1)^{w(w-1)/2}$ into $Q$; a consistent choice matters in weight two.

Fix $H_{\mathbb Z}$, $Q$ and the [Hodge numbers](../../../../../../hodge-number.md). The [compact dual of a period domain](../../../../../../compact-dual-of-a-period-domain.md) is the projective [flag variety](../../../../../../generalized-flag-variety.md)

$$
\check D=\left\{
F^\bullet:
\dim F^p=\sum_{r\ge p}h^{r,w-r},\
Q(F^p,F^{w-p+1})=0
\right\}.
$$

The orthogonality conditions are algebraic. The [Griffiths domain](../../../../../../period-domain.md) $D$ is the subset whose filtrations also satisfy real opposition and the displayed positivity. It is open in the usual complex topology of $\check D$; the inequalities are not additional complex algebraic equations. Thus **$\check D$ retains the complex flag conditions, whereas $D$ retains genuine [polarized Hodge structures](../../../../../../polarized-hodge-structure.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
