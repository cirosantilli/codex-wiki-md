<h1 id="10b/solution">Solution</h1>

↑ **Parent:** [10B](../10b.md)

On the smooth-function space, the product rule gives $ABf=(xf)'=f+xf'$ while $BAf=xf'$. Hence $\boxed{[A,B]=I}$, and both maps preserve the stated smooth space.

For general operators with this [commutator](../../../../../commutator.md) relation, use $[A,BC]=[A,B]C+B[A,C]$. Induction gives $[A,B^i]=iB^{i-1}$ for $i\geq1$. Since $Ay=0$,

$$
\boxed{A(By)=y,\qquad A(B^iy)=iB^{i-1}y\ (i\geq1),\qquad Ay=0.}
$$

Every displayed vector lies in $W$, so $W$ is invariant under $A$, as well as under $B$. Iterating the lowering formula gives $A^kB^iy=i!B^{i-k}y/(i-k)!$ for $k\leq i$, and zero for $k>i$.

Suppose a nontrivial finite [linear dependence](../../../../../linear-dependence.md) has highest nonzero term $c_nB^ny$. Applying $A^n$ kills all lower terms and yields $c_nn!y=0$. The field is real, $n!\ne0$, and $y\ne0$, so this contradicts $c_n\ne0$. Thus **the entire sequence is linearly independent**. This [identity commutator cyclic ladder](../../../../../identity-commutator-cyclic-ladder.md) also proves that such a representation with a nonzero vector in the kernel of $A$ cannot be finite dimensional.

## ↑ Ancestors (10)

1. [10B](../10b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
