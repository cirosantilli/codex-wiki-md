<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume first that $\mu(A\cap T^{-n}A)=0$ for every $n\geq1$. For $n>m$ the [measure-preserving transformation](../../../../../measure-preserving-transformation.md) property gives

$$
\mu(T^{-m}A\cap T^{-n}A)=\mu(A\cap T^{-(n-m)}A)=0.
$$

Thus the sets $T^{-n}A$, $n\geq0$, are pairwise disjoint and all have measure $\mu(A)>0$, impossible in a probability space. Hence

$$
\boxed{\mu(A\cap T^{-n}A)>0\text{ for some }n>0.}
$$

The [Poincaré recurrence theorem](../../../../../poincare-recurrence-theorem.md) states that almost every $x\in A$ returns to $A$ infinitely often. Let

$$
E=\{x\in A:T^nx\notin A\text{ for every }n\geq1\}.
$$

The sets $T^{-n}E$ are pairwise disjoint: if $x$ belonged to the $m$th and $n$th inverse images with $m<n$, then $T^mx\in E$ would return to $E\subseteq A$ after $n-m$ steps. Invariance and finiteness therefore give $\mu(E)=0$. A point of $A$ with only finitely many returns belongs, after its last return, to some $T^{-k}E$. The countable union of these null sets is null, proving the theorem.

Now let $S\subseteq\mathbb Z$ have $d^*(S)>0$. Put $x=\mathbf1_S\in\{0,1\}^{\mathbb Z}$ and let $\sigma$ be the bilateral shift. Choose intervals $I_j$ with $|I_j|\to\infty$ and $|S\cap I_j|/|I_j|\to d^*(S)$. A weak-star limit of

$$
\mu_j=\frac1{|I_j|}\sum_{m\in I_j}\delta_{\sigma^m x}
$$

exists on the compact shift space. Boundary terms show that the limit $\mu$ is $\sigma$-invariant. For the cylinder $A=\{y:y_0=1\}$,

$$
\mu(A)=d^*(S)>0.
$$

The stated polynomial recurrence theorem supplies $n>0$ with $\mu(A\cap\sigma^{-|P(n)|}A)>0$. Hence that cylinder intersection meets the orbit closure of $x$; because it is open, some shift $\sigma^m x$ lies in it. Therefore $m,m+|P(n)|\in S$. Orient these two integers according to the sign of $P(n)$ to obtain

$$
\boxed{a,b\in S\quad\text{and}\quad b-a=P(n).}
$$

This is the [Furstenberg correspondence principle](../../../../../furstenberg-correspondence-principle.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
