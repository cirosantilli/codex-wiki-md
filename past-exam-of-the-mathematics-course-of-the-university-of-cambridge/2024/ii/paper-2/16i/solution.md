<h1 id="16i/solution">Solution</h1>

↑ **Parent:** [16I](../16i.md)

The [Hartogs theorem](../../../../../hartogs-theorem.md) says that for every set $X$ there is an ordinal that does not inject into $X$. Indeed, the well-orderings of subsets of $X$ form a set, since each is a relation in $\mathcal P(X\times X)$. By replacement, their order types form a set of ordinals. Its supremum plus one cannot be the order type of a well-ordered subset of $X$, and hence cannot inject into $X$. The least such ordinal is the Hartogs ordinal $h(X)$.

[Ordinal exponentiation](../../../../../ordinal-exponentiation.md) is defined by

$$
\alpha^0=1,\qquad
\alpha^{\beta+1}=\alpha^\beta\alpha,\qquad
\alpha^\lambda=\sup_{\xi<\lambda}\alpha^\xi
$$

for nonzero [limit](../../../../../limit-of-a-function.md) $\lambda$. Fix $\alpha,\beta$ and induct on $\gamma$. The zero case is immediate. If the identity holds at $\gamma$, then

$$
\alpha^{\beta+(\gamma+1)}
=\alpha^{(\beta+\gamma)+1}
=\alpha^{\beta+\gamma}\alpha
=\alpha^\beta\alpha^{\gamma+1}.
$$

At a [limit](../../../../../limit-of-a-function.md) $\lambda$, continuity of exponentiation and right continuity of ordinal multiplication give

$$
\alpha^{\beta+\lambda}
=\sup_{\gamma<\lambda}\alpha^{\beta+\gamma}
=\sup_{\gamma<\lambda}\alpha^\beta\alpha^\gamma
=\alpha^\beta\alpha^\lambda.
$$

Put $\rho=\omega^\alpha$. The set

$$
B=\{\eta:\rho\eta\leq\gamma\}
$$

is nonempty and bounded, so let $\beta=\sup B$. Continuity of multiplication in its right argument gives $\rho\beta\leq\gamma$. There is a unique tail $\delta$ with $\gamma=\rho\beta+\delta$. If $\delta\geq\rho$, then  
$\rho(\beta+1)=\rho\beta+\rho\leq\gamma$, contrary to maximality. Hence $\delta<\rho$. If  
$\rho\beta+\delta=\rho\beta'+\delta'$ with both remainders below $\rho$ and $\beta<\beta'$, then

$$
\rho\beta+\delta<\rho(\beta+1)\leq\rho\beta',
$$

a contradiction. This proves existence and uniqueness in the [division by an additively indecomposable ordinal](../../../../../division-by-an-additively-indecomposable-ordinal.md).

Now let $X$ be nonempty and well ordered. Its least element is not a [limit](../../../../../limit-of-a-function.md) point, so $X'\ne X$. Every [derivative](../../../../../derivative.md) is itself a well-ordered subset. If $X^{(\alpha)}$ were nonempty for every $\alpha<h(X)$, then each difference

$$
X^{(\alpha)}\setminus X^{(\alpha+1)}
$$

would be nonempty. Choosing its least member would inject $h(X)$ into $X$, since the nested successive differences are disjoint. This contradicts Hartogs' lemma. Thus some [derivative](../../../../../derivative.md) is empty, as asserted by the [derived-set iteration of a well-order](../../../../../derived-set-iteration-of-a-well-order.md).

For an ordinal $\xi$, a point $\gamma<\xi$ is a [limit](../../../../../limit-of-a-function.md) point exactly when it is a nonzero [limit](../../../../../limit-of-a-function.md) ordinal. Division by $\omega$ writes $\gamma=\omega\beta+n$ with $n<\omega$; this is a nonzero [limit](../../../../../limit-of-a-function.md) exactly when $n=0$ and $\beta>0$. Hence

$$
\boxed{\xi'=\{\omega\beta<\xi:\beta>0\}}.
$$

Within this derived set, $\omega\beta$ is a [limit](../../../../../limit-of-a-function.md) point exactly when $\beta$ is a nonzero [limit](../../../../../limit-of-a-function.md) ordinal, equivalently $\beta=\omega\eta$ for some $\eta>0$. Therefore the [derived sets of an ordinal](../../../../../derived-sets-of-an-ordinal.md) satisfy

$$
\boxed{\xi''=\{\omega^2\eta<\xi:\eta>0\}}.
$$

Finally $\omega'=\varnothing$, so the index of $\omega$ is $1$, while  
$(\omega^2)'=\{\omega,2\omega,3\omega,\ldots\}$ and  
$(\omega^2)''=\varnothing$, so the index of $\omega^2$ is $2$.

## ↑ Ancestors (10)

1. [16I](../16i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
