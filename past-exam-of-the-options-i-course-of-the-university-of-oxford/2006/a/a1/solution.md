<h1 id="a/a1/solution">Solution</h1>

↑ **Parent:** [A1](../a1.md)

Write the [group action](../../../../group-action-split.md) as $(\omega,g)\mapsto\omega g$. A right [group action](../../../../group-action-split.md) satisfies $\omega1=\omega$ and $(\omega g)h=\omega(gh)$. Its [orbit](../../../../orbit-dynamical-system.md) and [stabilizer](../../../../stabilizer-subgroup.md) are

$$
\operatorname{Orb}(\omega)=\{\omega g:g\in G\},\qquad H=\operatorname{Stab}(\omega)=\{g\in G:\omega g=\omega\}.
$$

The identity belongs to $H$. If $g,h\in H$, then $\omega gh=(\omega g)h=\omega$, so $gh\in H$. Also $\omega g=\omega$ implies $\omega=(\omega g)g^{-1}=\omega g^{-1}$, so $g^{-1}\in H$. Thus $H$ is a [subgroup](../../../../subgroup.md).

For the [orbit-stabilizer theorem](../../../../orbit-stabilizer-theorem.md), the map $G\to\operatorname{Orb}(\omega)$, $g\mapsto\omega g$, is onto, and

$$
\omega g=\omega h\iff gh^{-1}\in H\iff g\in Hh.
$$

Its fibers are precisely the right [cosets](../../../../coset.md) $Hh$, each containing $|H|$ elements. Counting these disjoint fibers gives

$$
\boxed{|\operatorname{Orb}(\omega)|=|G|/|H|}.
$$

For the [symmetric group](../../../../symmetric-group.md) $S_3$, the six [subgroups](../../../../subgroup.md) are

$$
\{1\},\quad \langle(12)\rangle,\quad\langle(13)\rangle,\quad\langle(23)\rangle,\quad A_3=\{1,(123),(132)\},\quad S_3.
$$

The [group action](../../../../group-action-split.md) $H\mapsto g^{-1}Hg$ has **four orbits**: each of $\{1\}$, $A_3$, and $S_3$ is fixed, while the three order-two [subgroups](../../../../subgroup.md) form one [orbit](../../../../orbit-dynamical-system.md). Here an [orbit](../../../../orbit-dynamical-system.md) is a collection of [subgroups](../../../../subgroup.md), rather than a collection of individual permutations.

## ↑ Ancestors (12)

1. [A1](../a1.md)
2. [A](../../a.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
