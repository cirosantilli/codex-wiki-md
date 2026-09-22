<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use finite cutoff windows to avoid subtracting two infinite masses. Write $D$ for the unit disc, $D_U=\mathbf L_D\setminus\mathbf L_U$ on loops surrounding $0$, and $A(U)=\nu(D_U)$. For $0<r<1$, let $H_r=D_{rD}$. These increase to all loops in $\mathbf L_D$ surrounding $0$ as $r\downarrow0$.

On the finite-mass windows, the domain-containment events form a [pi-system](../../../../../../../pi-system.md). Indeed, if $U,V$ are simply connected and contain $0$, a simple loop surrounding $0$ that lies in both has its filled interior in both. It therefore lies in the component $W$ of $U\cap V$ containing $0$, which is simply connected. Thus, on the support of $\nu$,

$$
\mathbf L_U\cap\mathbf L_V=\mathbf L_W.
$$

[Inclusion-exclusion](../../../../../../../inclusion-exclusion-principle.md) for the finite deficits gives

$$
\nu(D_U\cap D_V)=A(U)+A(V)-A(W).
$$

Taking $V=rD$ and subtracting from $\nu(H_r)$ gives the useful recovery formula

$$
\boxed{\nu(H_r\cap\mathbf L_U)=A(W)-A(U),\qquad
W=\text{the component of }rD\cap U\text{ containing }0.}
$$

The assumed generation of the loop sigma-field by domain-containment events and the [uniqueness theorem for measures](../../../../../../../sigma-finite-uniqueness-theorem-for-measures.md) now determine the finite restriction to $H_r$. Increasing these windows recovers $\nu_D$; conformal transport recovers its restriction to any simply connected domain containing the marked point. If a simply connected domain omits $0$, no loop in it can surround $0$.

The argument uses finite annular deficits. This is the usual local-finiteness convention for these loop measures and is explicitly ensured by the finite logarithmic formula assumed in the continuation. Bare sigma-finiteness must not be used as permission for formal $\infty-\infty$ subtraction. This is the [recovery of a loop measure from conformal deficits](../../../../../../../recovery-of-a-loop-measure-from-conformal-deficits.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
