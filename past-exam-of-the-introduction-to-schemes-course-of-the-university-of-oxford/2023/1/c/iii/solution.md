<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $T=\operatorname{Spec}R$ and $Z=\operatorname{Spec}(R/(r))$. The [idempotent](../../../../../idempotent.md) $e$ determines the disjoint [clopen sets](../../../../../clopen-set.md) $Z_A=D_Z(e)$ and $Z_B=D_Z(1-e)$. Each is closed in $T$. Define the [open subsets](../../../../../open-set.md)

$$
T_A=T\setminus Z_B,\qquad T_B=T\setminus Z_A.
$$

They cover $T$ and satisfy $T_A\cap T_B=T\setminus Z=D(r)$. The [global section](../../../../../global-section.md) $r$ defines [morphisms of schemes](../../../../../morphism-of-schemes.md) $T_A\to A$ and $T_B\to B$, both sending the coordinate $t$ to $r$. On their intersection $r$ is a [unit](../../../../../unit-in-a-ring.md), so both maps land in the common [open subscheme](../../../../../open-subscheme.md) $A\cap B=\operatorname{Spec}\mathbb Z[t,t^{-1}]$, where they agree. They therefore glue uniquely:

$$
\boxed{u_{r,e}:T\longrightarrow X.}
$$

For an entirely explicit description, choose any lift $a\in R$ of $e$. Then $a(1-a)\in(r)$ and

$$
T_A=D(r)\cup D(a),\qquad T_B=D(r)\cup D(1-a).
$$

The equality $a+(1-a)=1$ proves that these [open subsets](../../../../../open-set.md) cover. The inclusion $D(a(1-a))\subseteq D(r)$ proves that their intersection is exactly $D(r)$. Their description as complements of $Z_A,Z_B$ proves independence of the chosen lift. In particular, no lift of $e$ to an [idempotent](../../../../../idempotent.md) of $R$ is required.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the introduction to schemes course of the University of Oxford](../../../../split.md)
6. [Introduction to schemes course of the University of Oxford](../../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
