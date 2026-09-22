<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Weak compactness of the adjoint forces weak compactness of the original operator.** Assume $T^*:Y^*\to X^*$ is weakly compact. Apply the already proved $(i)\Longrightarrow(ii)$ to this operator, rather than assuming the adjoint equivalence in advance. It gives

$$
T^{***}(Y^{***})\subseteq J_{X^*}(X^*).
$$

Take $\psi\in Y^{***}$ annihilating $J_YY$, so $\psi(J_Yy)=0$ for every $y\in Y$. Write $T^{***}\psi=J_{X^*}f$ for some $f\in X^*$. For every $x\in X$,

$$
f(x)=(J_{X^*}f)(J_Xx)=(T^{***}\psi)(J_Xx)
=\psi(T^{**}J_Xx)=\psi(J_YTx)=0.
$$

Hence $f=0$ and $T^{***}\psi=0$. It follows that

$$
\psi(T^{**}F)=0\qquad(F\in X^{**})
$$

for every $\psi$ annihilating $J_YY$.

The [vector subspace](../../../../../../vector-subspace.md) $J_YY$ is closed in the [norm topology](../../../../../../norm-topology.md) in $Y^{**}$ because $Y$ is complete and $J_Y$ is an [isometry](../../../../../../isometry.md). The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) says that any point outside a closed linear subspace can be separated from it by a [bounded linear functional](../../../../../../continuous-linear-functional.md) vanishing on that subspace. Applying this in $Y^{**}$ shows that an element annihilated by all such $\psi\in Y^{***}$ must belong to $J_YY$. Therefore $T^{**}F\in J_YY$ for every $F$, proving $(iv)\Longrightarrow(ii)$. The reverse implications above now establish all four equivalences, including [weak compactness of an operator and its adjoint](../../../../../../weak-compactness-of-an-operator-and-its-adjoint.md):

$$
\boxed{T\text{ weakly compact}\ \Longleftrightarrow\ T^{**}(X^{**})\subseteq J_YY
\ \Longleftrightarrow\ T^*\text{ is }w^*\text{-to-}w\text{ continuous}
\ \Longleftrightarrow\ T^*\text{ weakly compact}.}
$$

Finally, if $X$ is a [reflexive Banach space](../../../../../../reflexive-banach-space.md), every $F\in X^{**}$ is $J_Xx$ for some $x$, and $T^{**}F=J_YTx\in J_YY$. If $Y$ is a [reflexive Banach space](../../../../../../reflexive-banach-space.md), $Y^{**}=J_YY$, so the same range condition holds automatically. In either case, $(ii)\Longrightarrow(i)$ proves

$$
\boxed{X\text{ or }Y\text{ reflexive}\quad\Longrightarrow\quad\text{every bounded }T:X\to Y\text{ is weakly compact}.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
