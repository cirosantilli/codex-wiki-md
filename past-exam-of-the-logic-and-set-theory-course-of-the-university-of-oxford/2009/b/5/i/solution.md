<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) states that [injections](../../../../../injective-function.md) $f:A\to B$ and $g:B\to A$ imply the existence of a [bijection](../../../../../bijection.md) $A\to B$. Here is a direct proof, avoiding any appeal to a fixed-point theorem. Let $A_0=A\setminus g(B)$, $A_{n+1}=g(f(A_n))$, and $C=\bigcup_{n<\omega}A_n$. Define

$$
h(a)=\begin{cases}f(a),&a\in C,\\g^{-1}(a),&a\notin C.\end{cases}
$$

The second case is defined because $A\setminus C\subseteq g(B)$. On $C$, $f$ is a [bijection](../../../../../bijection.md) onto $f(C)$. For $b\in B$, injectivity of $g$ and the construction of $C$ give $g(b)\in C$ if and only if $b\in f(C)$: $g(b)$ cannot be in $A_0$, so membership in $C$ means membership in some $g(f(A_n))$. Hence $g^{-1}$ bijects $A\setminus C$ onto $B\setminus f(C)$. The two pieces have disjoint domains and images and together cover $A,B$, proving $h$ [bijective](../../../../../bijection.md). This proof itself uses no choice.

Write $\mathfrak c=|\mathbb R|=2^{\aleph_0}$. We use the standard infinite-cardinal identities $\kappa\cdot\aleph_0=\kappa$, $\kappa^n=\kappa$ for positive finite $n$ and infinite $\kappa$, and $(\kappa^\lambda)^\mu=\kappa^{\lambda\cdot\mu}$, under the permitted [axiom of choice](../../../../../axiom-of-choice.md). The map $z\mapsto(\operatorname{Re}z,\operatorname{Im}z)$ bijects $\mathbb C$ with $\mathbb R^2$. Therefore

$$
\boxed{|\mathbb C|=\mathfrak c^2=\mathfrak c.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
