<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We prove [Lie's theorem](../../../../../lie-s-theorem.md) in the required form by induction on $\dim L$. If $L=0$, any nonzero vector works. Otherwise solvability gives $[L,L]\ne L$, so choose a codimension-one ideal $K\supseteq[L,L]$ and $x\in L\setminus K$. By induction there are $v\ne0$ and a [linear functional](../../../../../linear-functional.md) $\lambda:K\to\mathbb C$ with $av=\lambda(a)v$ for all $a\in K$.

Let $W=\operatorname{span}\{v,xv,x^2v,\ldots\}$. Choose the cyclic [basis](../../../../../basis.md) $v,xv,\ldots,x^{r-1}v$ up to its first [linear dependence](../../../../../linear-dependence.md). The [commutator](../../../../../commutator.md) identity $ax^j=xax^{j-1}+[a,x]x^{j-1}$, with $[a,x]\in K$, proves inductively that

$$
ax^jv\equiv\lambda(a)x^jv\pmod{\operatorname{span}\{v,\ldots,x^{j-1}v\}}.
$$

Hence $W$ is invariant under $K$ and $x$, and every $a\in K$ has [trace](../../../../../matrix-trace.md) $r\lambda(a)$ on $W$. In particular $\operatorname{tr}_W([x,a])=0$ implies $r\lambda([x,a])=0$. [Characteristic zero](../../../../../characteristic-zero.md) gives $\lambda([x,a])=0$.

The simultaneous [weight space](../../../../../weight-space.md) $V_\lambda=\{w:aw=\lambda(a)w\ \forall a\in K\}$ is nonzero and stable under $x$, because

$$
a(xw)=x(aw)+[a,x]w=\lambda(a)xw.
$$

Over $\mathbb C$, the restriction of $x$ to this nonzero finite-dimensional space has an [eigenvector](../../../../../eigenvector.md). That vector is an [eigenvector](../../../../../eigenvector.md) of both $x$ and every $a\in K$, hence of every element of $L$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
