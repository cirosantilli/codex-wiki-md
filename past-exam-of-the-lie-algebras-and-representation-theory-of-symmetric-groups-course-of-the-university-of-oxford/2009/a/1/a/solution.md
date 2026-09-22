<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First prove the unlettered common-[eigenvector](../../../../../eigenvector.md) assertion, in the stronger form that some nonzero vector is killed by every operator in $W$. This is the linear form of [Engel's theorem](../../../../../engel-s-theorem.md).

Induct on $\dim W$, with the zero algebra immediate. If $a^r=0$, the operator $\operatorname{ad}a$ on $\operatorname{End}V$ is nilpotent: left and right multiplication commute, and every term in $(L_a-R_a)^{2r-1}$ contains a power of $a$ at least $r$. This argument works in every characteristic.

For a proper [Lie subalgebra](../../../../../lie-subalgebra.md) $H<W$, its action on $W/H$ by brackets is therefore by nilpotent operators. The image of this action has [dimension](../../../../../dimension-vector-space.md) at most $\dim H<\dim W$, so induction gives a nonzero class $w+H$ killed by $H$. Thus the normalizer $N_W(H)=\{w:[w,H]\subseteq H\}$ strictly contains $H$. Choose $H$ maximal proper. Its normalizer must be $W$, so $H$ is an ideal. Moreover $W/H$ has [dimension](../../../../../dimension-vector-space.md) one, since otherwise any one-dimensional subalgebra of the quotient would lift to an intermediate proper subalgebra.

Induction applied to $H$ acting on $V$ makes $V_0=\{v:Hv=0\}$ nonzero. This space is $W$-invariant: for $h\in H,x\in W,v\in V_0$, $h(xv)=x(hv)+[h,x]v=0$. Choose $x$ complementing $H$ in $W$. Its restriction to the nonzero space $V_0$ is nilpotent and has a nonzero kernel. A vector in this kernel is killed by $x$ and $H$, hence by all of $W$. This proves the preliminary assertion, with every common [eigenvalue](../../../../../eigenvalue.md) equal to zero.

Now apply it to the adjoint action of $L$ on itself. If $L\ne0$, its common zero space is the center $Z(L)$, which is therefore nonzero. Every induced adjoint map on $L/Z(L)$ remains nilpotent. Induction on [dimension](../../../../../dimension-vector-space.md) makes that quotient nilpotent. A central extension of a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) is nilpotent: if its lower central series vanishes after projection, the next term lies in the center and the following term is zero. Hence **$L$ is nilpotent**. The zero algebra is immediate.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
