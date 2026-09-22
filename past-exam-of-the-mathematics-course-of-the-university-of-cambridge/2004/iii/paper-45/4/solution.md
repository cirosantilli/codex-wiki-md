<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the finite-dimensional complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) setting, the [rank of a semisimple Lie algebra](../../../../../rank-of-a-semisimple-lie-algebra.md) is the dimension of a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak h$, equivalently the number of independent commuting Cartan generators. For a compact real algebra, use its complexification and the corresponding maximal torus. Simultaneously diagonalizing the commuting adjoint actions of $\mathfrak h$ gives the [root-space decomposition](../../../../../root-space-decomposition.md)

$$
\mathcal L=\mathfrak h\oplus\bigoplus_{\alpha\ne0}\mathcal L_\alpha,\qquad
\mathcal L_\alpha=\{X:[H,X]=\alpha(H)X\text{ for every }H\in\mathfrak h\}.
$$

The nonzero linear functionals $\alpha$ for which this space is nonzero are the [roots of a root system](../../../../../root-of-a-root-system.md). An invariant inner product identifies them with vectors in a real Euclidean root space. These are the usual semisimple assumptions behind the rank and root language here.

The displayed generators $H,E^+,E^-$ form an [sl2 triple](../../../../../sl2-triple.md). Start with a nonzero lowest-[weight](../../../../../weight-representation-theory.md) element $X_0$ and define $X_{n+1}=[E^+,X_n]$. The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
[H,X_{n+1}]=[[H,E^+],X_n]+[E^+,[H,X_n]].
$$

Induction starting with $[H,X_0]=-\lambda X_0$ consequently gives the [finite sl2 lowest-weight ladder](../../../../../finite-sl2-lowest-weight-ladder.md) [weights](../../../../../weight-representation-theory.md)

$$
\boxed{[H,X_n]=(2n-\lambda)X_n.}
$$

Now commute the lowering equation with $E^+$ and again use the [Jacobi identity](../../../../../jacobi-identity.md):

$$
[E^+,[E^-,X_n]]=[[E^+,E^-],X_n]+[E^-,[E^+,X_n]]
=(2n-\lambda)X_n+q_{n+1}X_n.
$$

The left side is $q_nX_n$. Whenever $X_n\ne0$, coefficient comparison gives

$$
\boxed{q_{n+1}=q_n+\lambda-2n.}
$$

The initial condition is $q_0=0$, meaning $[E^-,X_0]=0$; directly $[E^-,X_1]=[-H,X_0]=\lambda X_0$, so $q_1=\lambda$. Summing the recurrence from $0$ to $n-1$ yields

$$
\boxed{q_n=n\lambda-2\sum_{k=0}^{n-1}k=n(\lambda-n+1).}
$$

In fact the vector identity $[E^-,X_n]=n(\lambda-n+1)X_{n-1}$ follows inductively from the same [Jacobi identity](../../../../../jacobi-identity.md) without needing a separately assumed lowering coefficient.

If $X_{n_0}$ is the last nonzero element and $[E^+,X_{n_0}]=0$, apply $E^-$ to this zero next element. The lowering identity gives

$$
0=[E^-,X_{n_0+1}]=(n_0+1)(\lambda-n_0)X_{n_0},
$$

so **$\lambda=n_0$**, a nonnegative [integer](../../../../../integer.md). The nonzero endpoint is necessary. Literally allowing $X_{n_0}=0$ would make the printed conclusion false: take $X_0=E^-$ in the adjoint [representation](../../../../../group-representation.md) of $\mathfrak{sl}_2$. Then $\lambda=2$, $X_1=H$, $X_2=-2E^+$, $X_3=0$. Choosing $n_0=3$ gives a vanishing next bracket but not $\lambda=3$. The intended endpoint is the first terminating bracket after the nonzero ladder.

For the plus-sign nested [commutators](../../../../../commutator.md), use $H=H_1$, $E^\pm=E_1^\pm$ and $X_0=E_2^+$. The cross relation gives $[E_1^-,E_2^+]=0$, while $[H_1,E_2^+]=K_{21}E_2^+$. Thus the lowest-[weight](../../../../../weight-representation-theory.md) label is $\lambda=-K_{21}$. If the $n$-fold raised element is nonzero and the $(n+1)$-fold element vanishes, the preceding endpoint argument gives $\lambda=n$ and hence

$$
\boxed{K_{21}=-n.}
$$

For the minus-sign ladder, use the [sl2 triple](../../../../../sl2-triple.md) $H'=-H_1$, $E'^+=E_1^-$, $E'^-=E_1^+$ and start at $X_0=E_2^-$. Its lowest-[weight](../../../../../weight-representation-theory.md) equation is again $[H',X_0]=K_{21}X_0$, and its lowering bracket vanishes by the cross relation. The same argument proves exactly the same result, including the endpoint assumption that is explicit in the nested-[commutator](../../../../../commutator.md) question.

For arbitrary [roots of a root system](../../../../../root-of-a-root-system.md) $\alpha,\beta$, choose the normalized [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md) $\beta$, whose generators obey $[H_\beta,E_\beta^\pm]=\pm2E_\beta^\pm$ and $[E_\beta^+,E_\beta^-]=H_\beta$. The [coroot](../../../../../coroot.md) normalization gives

$$
\alpha(H_\beta)=\frac{2\alpha\cdot\beta}{\beta\cdot\beta}.
$$

The normalization has a concrete construction. Use the nondegenerate [Killing form](../../../../../killing-form.md) $B$, and define $t_\beta\in\mathfrak h$ by $B(t_\beta,H)=\beta(H)$. Invariance makes root spaces orthogonal unless their roots sum to zero, so there exist $e\in\mathcal L_\beta$ and $f\in\mathcal L_{-\beta}$ with $B(e,f)=1$. Invariance then gives $B([e,f],H)=B(e,[f,H])=\beta(H)$, hence $[e,f]=t_\beta$. With $(\beta,\beta)=\beta(t_\beta)$, take $E_\beta^+=e$, $E_\beta^-=2f/(\beta,\beta)$ and $H_\beta=2t_\beta/(\beta,\beta)$. Their brackets have the required normalization and $\alpha(H_\beta)=2(\alpha,\beta)/(\beta,\beta)$. Let $v$ be a nonzero $\alpha$ [root vector](../../../../../root-vector.md) with $H_\beta$ [weight](../../../../../weight-representation-theory.md) $w=\alpha(H_\beta)$. Repeatedly apply $\operatorname{ad}E_\beta^-$ until reaching a last nonzero vector $v_0=(\operatorname{ad}E_\beta^-)^pv$. Its [weight](../../../../../weight-representation-theory.md) is $w-2p$. This process terminates because different [weights](../../../../../weight-representation-theory.md) are linearly independent and the [Lie algebra](../../../../../lie-algebra-split.md) is finite-dimensional. Starting at $v_0$, repeatedly raise; this also terminates for the same reason. The proven lowest-[weight](../../../../../weight-representation-theory.md) endpoint formula says $w-2p=-N$ for a nonnegative integer $N$. Therefore

$$
\boxed{\frac{2\alpha\cdot\beta}{\beta^2}=w=2p-N\in\mathbb Z.}
$$

This proves integrality of [Cartan integers](../../../../../cartan-integer.md) directly from the finite ladder, rather than assuming the crystallographic axiom.

Finally use the indices actually printed in the PDF: $E_1^+=R^1{}_2$, $E_2^+=R^2{}_3$, $E_1^-=R^2{}_1$, $E_2^-=R^3{}_2$. The converted TeX has corrupted these indices. The prescribed bracket is that of trace-free [matrix units](../../../../../matrix-unit.md). The sum of the diagonal generators is zero, leaving two independent diagonal elements, and their pair brackets give

$$
\boxed{H_1=R^1{}_1-R^2{}_2,\qquad H_2=R^2{}_2-R^3{}_3.}
$$

For example $[R^1{}_2,R^2{}_1]=R^1{}_1-R^2{}_2$, and the analogous second pair gives $H_2$. The cross raising-lowering brackets vanish. A diagonal $H$ with entries $h_r$ has $[H,R^r{}_s]=(h_r-h_s)R^r{}_s$. Thus $H_1$ acts on $E_1^+,E_2^+$ with [weights](../../../../../weight-representation-theory.md) $2,-1$, and $H_2$ acts on them with [weights](../../../../../weight-representation-theory.md) $-1,2$. The negative generators have the opposite [weights](../../../../../weight-representation-theory.md). In the question's index ordering,

$$
\boxed{(K_{ji})=\begin{pmatrix}2&-1\\-1&2\end{pmatrix}.}
$$

This is the [Cartan matrix](../../../../../cartan-matrix.md) of the [A2 root system](../../../../../a2-root-system.md), and the [Lie algebra](../../../../../lie-algebra-split.md) generated by these matrix units has rank two. As an additional bracket check, $[E_1^+,E_2^+]=R^1{}_3\ne0$ whereas $[E_1^+,R^1{}_3]=0$, so the nested ladder has $n=1$ and indeed $K_{21}=-1$. The negative ladder likewise terminates after one nonzero bracket.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
