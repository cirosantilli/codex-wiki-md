<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First use the nonzero loci, as required by the standard [SL2R action on differentials](../../../../../../sl2r-action-on-differentials.md). A nonzero [holomorphic one-form](../../../../../../holomorphic-one-form.md) has, away from its zeros, [flat coordinates](../../../../../../natural-coordinate-of-a-holomorphic-differential.md)

$$
w=\int\omega,\qquad\omega=dw,
$$

whose changes of coordinate are translations. A nonzero [holomorphic quadratic differential](../../../../../../holomorphic-quadratic-differential.md) similarly has local [flat coordinates](../../../../../../natural-coordinate-of-a-holomorphic-differential.md) $w=\int\sqrt q$, with $q=dw^2$ and changes of coordinate $w_j=\pm w_i+c_{ij}$. These are respectively [translation surfaces](../../../../../../translation-surface.md) and [half-translation surfaces](../../../../../../half-translation-surface.md).

Identify a [flat coordinate](../../../../../../natural-coordinate-of-a-holomorphic-differential.md) with a vector in $\mathbb R^2$. For $A\in\mathrm{SL}_2(\mathbb R)$, replace every [flat coordinate](../../../../../../natural-coordinate-of-a-holomorphic-differential.md) by $W=Aw$. Since $A$ preserves [orientation](../../../../../../orientation-of-a-simplex.md) and commutes with multiplication by $-1$, the new changes of coordinate are

$$
W_j=W_i+Ac_{ij},\qquad\text{or}\qquad W_j=\pm W_i+Ac_{ij}.
$$

They are [holomorphic](../../../../../../complex-differentiability-at-a-point.md) in the new coordinates, and so define a new [complex structure](../../../../../../complex-structure.md). Define $\omega_A=dW$ or $q_A=dW^2$ in that structure. The forms glue because translations preserve $dW$, and the extra signs preserve $dW^2$.

The zeros also extend. A zero of order $m$ of a [holomorphic one-form](../../../../../../holomorphic-one-form.md) has [cone angle](../../../../../../cone-angle.md) $2\pi(m+1)$; a zero of order $m$ of a [holomorphic quadratic differential](../../../../../../holomorphic-quadratic-differential.md) has [cone angle](../../../../../../cone-angle.md) $(m+2)\pi$. The real-linear deformation preserves the corresponding winding multiplicity. Filling the cone in a local coordinate $\zeta$ gives $W=\zeta^{m+1}$ in the first case, or a local branch of $W=\zeta^{(m+2)/2}$ in the second. Thus the resulting forms are constant multiples of $\zeta^m\,d\zeta$ or $\zeta^m\,d\zeta^2$ and have the same [zero orders](../../../../../../order-of-a-zero-of-a-differential.md). This verifies extension across the missing points, rather than merely producing an atlas on the punctured surface.

An isomorphism preserving the original differential identifies its [flat coordinates](../../../../../../natural-coordinate-of-a-holomorphic-differential.md) up to the permitted translations or signs; applying $A$ identifies the deformed atlases too. Hence the construction descends to the corresponding [moduli spaces](../../../../../../moduli-space.md). Applying $B$ after $A$ replaces $w$ by $BAw$, so

$$
\boxed{B\cdot(A\cdot(X,\omega))=(BA)\cdot(X,\omega),\qquad
B\cdot(A\cdot(X,q))=(BA)\cdot(X,q).}
$$

The [area of a quadratic differential](../../../../../../area-of-a-quadratic-differential.md), and the analogous area of a [holomorphic one-form](../../../../../../holomorphic-one-form.md), are preserved because $\det A=1$.

For $q=\omega^2$, the [flat coordinates](../../../../../../natural-coordinate-of-a-holomorphic-differential.md) obtained from $\omega$ already give the required [half-translation surface](../../../../../../half-translation-surface.md) atlas for $q$. The same replacement $w\mapsto Aw$ therefore constructs both deformations, and

$$
\boxed{A\cdot(X,\omega^2)=(X_A,\omega_A^2)=s\bigl(A\cdot(X,\omega)\bigr).}
$$

The printed sets include identically zero differentials. They have no [flat coordinates](../../../../../../natural-coordinate-of-a-holomorphic-differential.md), so the customary geometric [group action](../../../../../../group-action.md) is defined on the nonzero loci. One can obtain a set-theoretic action on the displayed entire sets by declaring $A\cdot(X,0)=(X,0)$; the same equivariance identity then holds at zero. This extension is generally not continuous: as $t\omega\to0$, the deformed underlying surface is the same $X_A$ for every real $t>0$, and can differ from $X$. Thus a claim about the standard continuous geometric [group action](../../../../../../group-action.md) requires the nonzero convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
