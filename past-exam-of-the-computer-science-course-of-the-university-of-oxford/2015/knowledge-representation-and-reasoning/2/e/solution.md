<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The standard semantics of [ALC](../../../../../alc.md) and [EL](../../../../../el.md) do not impose the [unique name assumption](../../../../../unique-name-assumption.md). Therefore the two individual names may denote the same element. A minimum-size model of either normalized [TBox](../../../../../tbox.md) from part (d), together with the [ABox](../../../../../abox.md), is

$$
\boxed{\begin{gathered}
\Delta^{\mathcal I}=\{d\},\qquad a^{\mathcal I}=b^{\mathcal I}=d,\\
A^{\mathcal I}=C^{\mathcal I}=X^{\mathcal I}=\{d\},\qquad B^{\mathcal I}=\varnothing,\\
R^{\mathcal I}=P^{\mathcal I}=\{(d,d)\}.
\end{gathered}}
$$

The $R$ self-loop supplies the [ABox](../../../../../abox.md) fact and makes both $\exists R.A$ and $\exists R.X$ true at $d$. The $P$ self-loop supplies exactly the existential restriction defining $C$. Disjointness holds because $B$ is empty. Hence every normalized [general concept inclusion](../../../../../general-concept-inclusion.md) is satisfied. A domain must be nonempty, so $\boxed{|\Delta^{\mathcal I}|=1}$ is minimal.

If a separate [unique name assumption](../../../../../unique-name-assumption.md) were imposed, the minimum would instead be two. One can take $a\ne b$, $A=\{a\}$, $C=\{b\}$, $R=\{(a,b)\}$, $P=\{(b,b)\}$ and $B=X=\varnothing$. There is then no $R$-edge ending at an $A$ element, so the normalized requirements involving $X$ hold vacuously. That additional convention is not part of standard [description logic](../../../../../description-logic.md) semantics.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
