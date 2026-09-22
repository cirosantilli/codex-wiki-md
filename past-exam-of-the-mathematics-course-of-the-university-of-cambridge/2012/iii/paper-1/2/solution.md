<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md)

$$
L^{(0)}=L,\qquad L^{(r+1)}=[L^{(r)},L^{(r)}].
$$

A [solvable Lie algebra](../../../../../solvable-lie-algebra.md) has $L^{(r)}=0$ for some $r$. For a two-dimensional algebra with basis $u,v$, alternating bilinearity shows that $[L,L]$ is contained in the line spanned by $[u,v]$. A one-dimensional [Lie algebra](../../../../../lie-algebra-split.md) is abelian, so $[[L,L],[L,L]]=0$. **Every two-dimensional complex [Lie algebra](../../../../../lie-algebra-split.md) is solvable, with derived length at most two.** This dimension argument actually works over any field with the alternating definition of a [Lie bracket](../../../../../lie-bracket.md).

There is a genuine qualification in the last request: the assertion about all [Irreducible Lie algebra representations](../../../../../irreducible-lie-algebra-representation.md) is true for finite-dimensional representations. Without that restriction, the [infinite-dimensional simple module for the two-dimensional affine Lie algebra](../../../../../infinite-dimensional-simple-module-for-the-two-dimensional-affine-lie-algebra.md) is a counterexample. Take $L=\mathbb Cx\oplus\mathbb Cy$, with $[x,y]=y$, and let it act on $V=\mathbb C[t]$ by

$$
(xf)(t)=tf(t),\qquad(yf)(t)=f(t-1).
$$

Then $[x,y]f=tf(t-1)-(t-1)f(t-1)=yf$, so this is a [Lie algebra representation](../../../../../lie-algebra-representation.md). Any nonzero [submodule](../../../../../submodule.md) is stable under multiplication by $t$, hence is an ideal $p(t)\mathbb C[t]$. Stability under $y$ implies $p(t)\mid p(t-1)$. The two [polynomials](../../../../../polynomial-split.md) have the same degree; their leading coefficients also agree, so $p(t-1)=p(t)$. In characteristic zero this forces $p$ to be constant. Thus $V$ is infinite-dimensional and irreducible, while $L$ is solvable. **The literal unrestricted assertion is false.**

Here is a proof of the intended finite-dimensional assertion, including the essential [Lie theorem](../../../../../lie-s-theorem.md) argument. We prove that a nonzero finite-dimensional representation $\rho:L\to\operatorname{End}(V)$ of a complex solvable algebra has a common [eigenvector](../../../../../eigenvector.md), by induction on $\dim L$. If $L=0$, any nonzero vector works. Otherwise $[L,L]\ne L$; choose a hyperplane $K$ containing $[L,L]$. It is a solvable ideal, and $L=K\oplus\mathbb Cx$. Induction gives $v\ne0$ and $\lambda\in K^*$ with $\rho(y)v=\lambda(y)v$ for all $y\in K$. Write $X=\rho(x)$ and suppress $\rho$ on elements of $K$.

Let $v_j=X^jv$ and let $m$ be the first index for which $v_m$ lies in the span of $v_0,\ldots,v_{m-1}$. The space $W=\operatorname{span}(v_0,\ldots,v_{m-1})$ is $X$-invariant. Repeatedly using $yX=Xy+[y,x]$ and $[y,x]\in K$ proves inductively that

$$
yv_j-\lambda(y)v_j\in\operatorname{span}(v_0,\ldots,v_{j-1}).
$$

Thus $W$ is $K$-invariant, and every $y\in K$ has constant diagonal $\lambda(y)$ in this basis. The [trace](../../../../../matrix-trace.md) of a [commutator](../../../../../commutator.md) is zero, so

$$
0=\operatorname{tr}_W[X,y]=m\lambda([x,y]).
$$

Since we work over $\mathbb C$, $\lambda([x,y])=0$ for all $y\in K$. Therefore the nonzero simultaneous [eigenspace](../../../../../eigenspace.md)

$$
V_\lambda=\{w\in V:yw=\lambda(y)w\text{ for every }y\in K\}
$$

is $X$-invariant: $yXw=\lambda(y)Xw+\lambda([y,x])w=\lambda(y)Xw$. A complex linear operator on a nonzero finite-dimensional space has an [eigenvector](../../../../../eigenvector.md). An [eigenvector](../../../../../eigenvector.md) of $X|_{V_\lambda}$ is consequently a common [eigenvector](../../../../../eigenvector.md) for $L$.

Its span is a one-dimensional [submodule](../../../../../submodule.md). If $V$ is irreducible, that span must be all of $V$. Hence **every finite-dimensional irreducible representation of a finite-dimensional complex solvable [Lie algebra](../../../../../lie-algebra-split.md) has dimension one**. Conversely a one-dimensional representation is given by a [linear functional](../../../../../linear-functional.md) on $L/[L,L]$, because every [commutator](../../../../../commutator.md) acts by zero. Passing repeatedly to quotients also gives the [simultaneous triangularization of a Lie algebra representation](../../../../../simultaneous-triangularization-of-a-lie-algebra-representation.md). Neither the [eigenvector](../../../../../eigenvector.md) step nor the [trace](../../../../../matrix-trace.md) argument extends to the infinite-dimensional counterexample above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
