<h1 id="4/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use only the definability and truth clauses of the [forcing theorem](../../../../../../../forcing-theorem.md). For every formula, its [forcing](../../../../../../../forcing-split.md) relation on names is definable inside $M$; [forcing](../../../../../../../forcing-split.md) is preserved by strengthening; and $M[G]\models\varphi(\vec\tau^G)$ exactly when some condition in $G$ forces $\varphi(\vec\tau)$. These clauses do not presuppose the Separation axiom we are proving.

Let $a=\tau^G$ and let $\vec\sigma^G$ be the parameters in the desired instance. In $M$, form the name

$$
\rho=\{(\nu,q):\exists p\,[(\nu,p)\in\tau\ \land\ q\ge p
\ \land\ q\Vdash\varphi(\nu,\vec\sigma)]\}.
$$

This is a set in $M$ by its Separation axiom and [forcing](../../../../../../../forcing-split.md) definability, using the subnames of $\tau$ and $P$ as a set-sized bound.

If $x\in\rho^G$, some $q\in G$ activates $(\nu,q)$ and $q\ge p$ activates $(\nu,p)\in\tau$. Thus $x=\nu^G\in a$, and the [forcing](../../../../../../../forcing-split.md) theorem gives $\varphi(x,\vec\sigma^G)$. Conversely, if $x\in a$ satisfies that formula, choose an active pair $(\nu,p)\in\tau$ with $x=\nu^G$ and a condition $r\in G$ [forcing](../../../../../../../forcing-split.md) the formula. Directedness gives $q\in G$ stronger than both $p$ and $r$. Monotonicity puts $(\nu,q)\in\rho$, so $x\in\rho^G$.

Therefore

$$
\boxed{\rho^G=\{x\in a:M[G]\models\varphi(x,\vec\sigma^G)\}.}
$$

Every requested instance of [separation in a generic extension](../../../../../../../separation-in-a-generic-extension.md) follows.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [4](../../../4.md)
4. [Paper 19](../../../../paper-19-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
