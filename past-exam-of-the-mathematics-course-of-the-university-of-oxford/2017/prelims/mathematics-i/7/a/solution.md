<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A left [group action](../../../../../../group-action-split.md) is a map $a:G\times X\to X$ satisfying

$$
a(e,x)=x,\qquad a(gh,x)=a\bigl(g,a(h,x)\bigr)
\quad(g,h\in G,\ x\in X).
$$

Define $\rho_a(g):X\to X$ by $\rho_a(g)(x)=a(g,x)$. The action axioms give

$$
\rho_a(g)\circ\rho_a(g^{-1})=\rho_a(e)=\operatorname{id}_X
=\rho_a(g^{-1})\circ\rho_a(g).
$$

Hence each $\rho_a(g)$ is a [bijection](../../../../../../bijection.md), with inverse $\rho_a(g^{-1})$, and belongs to the [symmetric group](../../../../../../symmetric-group.md) $\operatorname{Sym}(X)$. Finally,

$$
\rho_a(gh)(x)=a(gh,x)=a\bigl(g,a(h,x)\bigr)
=\bigl(\rho_a(g)\circ\rho_a(h)\bigr)(x),
$$

so $\rho_a:G\to\operatorname{Sym}(X)$ is a [group homomorphism](../../../../../../group-homomorphism.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
