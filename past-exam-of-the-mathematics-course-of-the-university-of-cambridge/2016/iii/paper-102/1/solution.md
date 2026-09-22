<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Over the complex numbers, every finite-dimensional representation of a solvable Lie algebra has a basis in which every representing matrix is upper triangular.** The [Lie theorem](../../../../../lie-s-theorem.md) is often stated first as the existence of a common [eigenvector](../../../../../eigenvector.md) in every nonzero finite-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md) of a [solvable Lie algebra](../../../../../solvable-lie-algebra.md). Applying that assertion successively to [quotient representations](../../../../../quotient-representation.md) gives an invariant [complete flag](../../../../../complete-flag.md), and hence the upper triangular form. The same proof works over any [algebraically closed field](../../../../../algebraically-closed-field.md) of [characteristic zero](../../../../../characteristic-zero.md).

We prove the common [eigenvector](../../../../../eigenvector.md) assertion by induction on $\dim\mathfrak g$, writing the action as $av$. The zero [Lie algebra](../../../../../lie-algebra-split.md) is immediate. If $\mathfrak g\ne0$ is [solvable](../../../../../solvable-lie-algebra.md), its [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) shows that $[\mathfrak g,\mathfrak g]\ne\mathfrak g$. Choose a codimension-one [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) $\mathfrak a$ containing $[\mathfrak g,\mathfrak g]$, and choose $x\notin\mathfrak a$. By induction there are $v\ne0$ and a [linear functional](../../../../../linear-functional.md) $\lambda:\mathfrak a\to\mathbb C$ such that $av=\lambda(a)v$ for all $a\in\mathfrak a$.

Let $W$ be the span of $v,xv,x^2v,\ldots$. If $m=\dim W$, the first $m$ of these vectors form a [basis](../../../../../basis.md), and $W$ is $x$-invariant. We claim that for each $a\in\mathfrak a$,

$$
a x^jv=\lambda(a)x^jv+\operatorname{span}\{v,xv,\ldots,x^{j-1}v\}.
$$

For $j=0$ this is the definition of $v$. For the induction step, use $ax=x a+[a,x]$ and $[a,x]\in\mathfrak a$. Applying the induction hypothesis to both $a$ and $[a,x]$ proves the claim. Consequently $W$ is $\mathfrak a$-invariant, and every $a\in\mathfrak a$ acts on $W$ by an upper triangular [matrix](../../../../../matrix.md) with all diagonal entries $\lambda(a)$.

Since both $x$ and $a$ preserve $W$, the [matrix trace](../../../../../matrix-trace.md) of their [commutator](../../../../../commutator.md) on $W$ is zero. The claim applied to $[x,a]\in\mathfrak a$ gives

$$
0=\operatorname{tr}_W[x,a]=m\lambda([x,a]).
$$

Here [characteristic zero](../../../../../characteristic-zero.md) is essential: $m\ne0$ in the field, so $\lambda([x,a])=0$. Now the common [weight space](../../../../../weight-space.md)

$$
E_\lambda=\{w\in V:aw=\lambda(a)w\text{ for all }a\in\mathfrak a\}
$$

is nonzero and $x$-invariant. Indeed, for $w\in E_\lambda$,

$$
a(xw)=x(aw)+[a,x]w=\lambda(a)xw+\lambda([a,x])w=\lambda(a)xw.
$$

An endomorphism of a nonzero finite-dimensional complex [vector space](../../../../../vector-space-split.md) has an [eigenvector](../../../../../eigenvector.md), so choose an [eigenvector](../../../../../eigenvector.md) of $x$ in $E_\lambda$. It is a common [eigenvector](../../../../../eigenvector.md) for $\mathfrak g=\mathfrak a+\mathbb Cx$. This proves the [Lie theorem](../../../../../lie-s-theorem.md).

**For the printed matrices in characteristic $p$, $[x,y]=x$, and there is no common eigenvector.** Index the standard [basis](../../../../../basis.md) by $e_0,\ldots,e_{p-1}$. The cyclic entry in the PDF gives

$$
x e_j=e_{j-1}\quad(j\text{ modulo }p),\qquad ye_j=je_j.
$$

The $p$ diagonal [eigenvalues](../../../../../eigenvalue.md) of $y$ are distinct in $k$. Thus every [eigenvector](../../../../../eigenvector.md) of $y$ is a scalar multiple of a single $e_j$. Since $p\ge2$, $xe_j$ is never a scalar multiple of $e_j$, proving the assertion even when $k$ is not an [algebraically closed field](../../../../../algebraically-closed-field.md).

For $1\le j\le p-1$,

$$
[x,y]e_j=j e_{j-1}-(j-1)e_{j-1}=e_{j-1}.
$$

At the cyclic boundary,

$$
[x,y]e_0=-(p-1)e_{p-1}=e_{p-1}.
$$

Hence $[x,y]=x$. The two-dimensional [Lie subalgebra](../../../../../lie-subalgebra.md) $kx+ky$ has [derived algebra](../../../../../derived-algebra.md) $kx$, whose own [derived algebra](../../../../../derived-algebra.md) is zero, so it is [solvable](../../../../../solvable-lie-algebra.md). It nevertheless has no common [eigenvector](../../../../../eigenvector.md), including after extending $k$ to its [algebraic closure](../../../../../algebraic-closure.md). This is a [failure of Lie theorem in positive characteristic](../../../../../failure-of-lie-theorem-in-positive-characteristic.md). In the proof above, the obstruction is precisely that $\dim W=p$ can vanish as a scalar in $k$.

**The derived algebra of a complex solvable Lie algebra is nilpotent.** First suppose $\mathfrak g\subseteq\mathfrak{gl}(V)$. By the [Lie theorem](../../../../../lie-s-theorem.md), put every element of $\mathfrak g$ in upper triangular form. The diagonal of a [commutator](../../../../../commutator.md) of upper triangular [matrices](../../../../../matrix.md) is zero, so $\mathfrak d=[\mathfrak g,\mathfrak g]$ consists of strictly upper triangular [matrices](../../../../../matrix.md). The [Lie algebra](../../../../../lie-algebra-split.md) of all such [matrices](../../../../../matrix.md) is a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md): if $F_r$ consists of [matrices](../../../../../matrix.md) whose entries vanish whenever $j-i<r$, then

$$
[F_r,F_s]\subseteq F_{r+s},\qquad F_{\dim V}=0.
$$

Therefore the [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) of $\mathfrak d$ reaches zero. Alternatively, every element of $\mathfrak d$ is a [nilpotent linear map](../../../../../nilpotent-linear-map.md), and the [Engel theorem](../../../../../engel-s-theorem.md) states that a finite-dimensional [Lie subalgebra](../../../../../lie-subalgebra.md) consisting of [nilpotent linear maps](../../../../../nilpotent-linear-map.md) is a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md).

For an abstract complex [solvable Lie algebra](../../../../../solvable-lie-algebra.md) $\mathfrak g$, apply the preceding result to its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). The [Lie algebra](../../../../../lie-algebra-split.md) $\operatorname{ad}\mathfrak d=[\operatorname{ad}\mathfrak g,\operatorname{ad}\mathfrak g]$ is [nilpotent](../../../../../nilpotent-lie-algebra.md). Since $\ker(\operatorname{ad}|_{\mathfrak d})=\mathfrak d\cap Z(\mathfrak g)$ is central in $\mathfrak d$, some term of the [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) of $\mathfrak d$ lies in that central [ideal](../../../../../ideal.md); the next term is zero. Thus $\mathfrak d$ itself is [nilpotent](../../../../../nilpotent-lie-algebra.md).

Conversely, every [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) is [solvable](../../../../../solvable-lie-algebra.md), since its [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) is contained term by term in its [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md). If $\mathfrak d$ is [nilpotent](../../../../../nilpotent-lie-algebra.md), it is therefore [solvable](../../../../../solvable-lie-algebra.md), and $\mathfrak g/\mathfrak d$ is [Abelian](../../../../../abelian-group.md). More directly, the [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) of $\mathfrak g$, after its first term, is the [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) of $\mathfrak d$. Consequently the [derived algebra nilpotence criterion](../../../../../derived-algebra-nilpotence-criterion.md) is

$$
\boxed{\mathfrak g\text{ solvable}\quad\Longleftrightarrow\quad[\mathfrak g,\mathfrak g]\text{ nilpotent}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
