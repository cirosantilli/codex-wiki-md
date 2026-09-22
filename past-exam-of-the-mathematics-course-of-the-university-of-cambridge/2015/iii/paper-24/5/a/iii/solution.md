<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [diamond-sequence forcing](../../../../../../../diamond-sequence-forcing.md). A condition is a sequence

$$
p=\langle A_\xi:\xi\leq\delta_p\rangle,qquad
\delta_p<\omega_1,\quad A_\xi\subseteq\xi,
$$

ordered by end extension. Its countable descending chains have lower bounds: take their union and, if their lengths approach a new limit, add an arbitrary subset at that last index. Hence it is [countably closed](../../../../../../../countably-closed-forcing.md) and preserves $\omega_1$. The union of the [generic filter](../../../../../../../generic-filter.md) supplies $\langle A_\xi:\xi<\omega_1\rangle$.

To prove the [diamond principle](../../../../../../../diamond-principle.md), let a condition force that $\dot X\subseteq\omega_1$ and that $\dot C$ is a [club set](../../../../../../../club-set.md). Below any such condition build $p_n$ and strictly increasing countable ordinals $\delta_n$ so that $\delta_n>\delta_{p_n}$, $p_{n+1}$ forces $\delta_n\in\dot C$, decides $\dot X\cap\delta_n$, and has length past $\delta_n$. Unboundedness supplies $\delta_n$; countable closure allows deciding all the bits below it. The construction can be carried out in $M$.

Let $\delta=\sup_n\delta_n=\sup_n\delta_{p_n}$. The union of the conditions has entries exactly below $\delta$ and decides a ground-model set $x=\dot X\cap\delta$. Extend that union by setting $A_\delta=x$. This condition forces $\delta\in\dot C$ by closure, and $A_\delta=\dot X\cap\delta$. The conditions giving a correct guess inside any named [club set](../../../../../../../club-set.md) are therefore dense. Thus

$$
\boxed{M[G]\models\diamondsuit.}
$$

No ground-model [Continuum hypothesis](../../../../../../../continuum-hypothesis.md) is needed; this forcing is allowed to collapse higher cardinals.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
