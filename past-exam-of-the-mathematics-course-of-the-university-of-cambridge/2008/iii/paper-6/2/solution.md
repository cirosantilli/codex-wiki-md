<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [special linear group](../../../../../special-linear-group.md) $G=\mathrm{SL}_3(\overline{\mathbb F}_q)$, let $N=q-1$, and choose a generator $\chi$ of the [character group](../../../../../character-group.md) of $\mathbb F_q^\times$. Every [linear character](../../../../../linear-character.md) of the diagonal [rational maximal torus](../../../../../rational-maximal-torus.md) has a unique expression

$$
\theta\bigl(\operatorname{diag}(a,b,(ab)^{-1})\bigr)=\chi(a)^r\chi(b)^s,\qquad r,s\in\mathbb Z/N\mathbb Z.
$$

The upper triangular [Borel subgroup](../../../../../borel-subgroup.md) $B=TU$ is rational. Consequently its [Deligne-Lusztig induction](../../../../../deligne-lusztig-induction.md) is the actual [principal series of a finite reductive group](../../../../../principal-series-of-a-finite-reductive-group.md)

$$
R_T^G(\theta)=\operatorname{Ind}_{B^F}^{G^F}\widetilde\theta,
$$

where $\widetilde\theta$ is the [inflation of a group representation](../../../../../inflation-of-a-group-representation.md) across $B^F\to T^F$. The geometric reason for this split case is $X(1)=G^F/B^F$: the associated torus covering supplies $\theta$, and the auxiliary unipotent fibres contribute a single even cohomological degree, hence no minus sign.

The rational [Bruhat decomposition](../../../../../bruhat-decomposition.md) indexes $B^F\backslash G^F/B^F$ by $W=S_3$. Applying the [Mackey restriction formula](../../../../../mackey-restriction-formula.md) and [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) gives

$$
\left\langle R_T^G(\theta),R_T^G(\theta)\right\rangle_{G^F}=\sum_{w\in S_3}\dim\operatorname{Hom}_{B^F\cap{}^{\dot w}B^F}\bigl(\widetilde\theta,{}^{\dot w}\widetilde\theta\bigr)=|\operatorname{Stab}_{S_3}(\theta)|.
$$

Each intersection contains $T^F$, and the two [linear characters](../../../../../linear-character.md) are trivial on its unipotent part. Its contribution is therefore one exactly when $w$ fixes $\theta$, and zero otherwise. Complete reducibility over $\mathbb C$ makes this [character inner product](../../../../../character-inner-product.md) the sum of squares of [irreducible representation](../../../../../irreducible-representation.md) multiplicities. Thus the [principal series of a finite reductive group](../../../../../principal-series-of-a-finite-reductive-group.md) is irreducible exactly when the [Weyl group](../../../../../weyl-group.md) stabilizer is trivial.

To compute that stabilizer, represent $\theta$ by the triple $(\chi^r,\chi^s,1)$. Two triples give the same [linear character](../../../../../linear-character.md) on determinant-one diagonal matrices exactly when they differ by a common factor $(\nu,\nu,\nu)$. For example, triviality of $(\eta_1,\eta_2,\eta_3)$ on all such matrices first gives $\eta_1=\eta_3$ by varying $a$, and then $\eta_2=\eta_3$ by varying $b$. The [Weyl group](../../../../../weyl-group.md) permutes the three entries.

A transposition fixes $\theta$ precisely when its two interchanged entries coincide: the third, fixed entry forces the common factor to be one. These three obstructions are $r=0$, $s=0$, and $r=s$. A three-cycle can also fix $\theta$ without any two entries coinciding. Its common factor must satisfy $\nu^3=1$; in the nontrivial case the entries, up to order and common factor, are $(1,\nu,\nu^2)$. This happens exactly when $3\mid N$ and $\{r,s\}=\{N/3,2N/3\}$.

The complete condition is therefore

$$
\boxed{r\not\equiv0,\quad s\not\equiv0,\quad r-s\not\equiv0\pmod N,\qquad 3\mid N\Longrightarrow\{r,s\}\ne\{N/3,2N/3\}.}
$$

In particular **pairwise distinct coordinate characters alone are insufficient**. For $q=4$ the only distinct triples have the order-three symmetry, and no character of this split [rational maximal torus](../../../../../rational-maximal-torus.md) gives an irreducible [principal series of a finite reductive group](../../../../../principal-series-of-a-finite-reductive-group.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
