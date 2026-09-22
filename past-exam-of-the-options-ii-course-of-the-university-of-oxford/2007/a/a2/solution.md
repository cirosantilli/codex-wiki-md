<h1 id="a/a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

Every nonzero vector can be extended to a [basis](../../../../basis.md), and the invertible map between two such bases carries the first vector to the second. The action is therefore transitive. Counting ordered bases gives

$$
|G|=(8-1)(8-2)(8-4)=168.
$$

The [stabilizer](../../../../stabilizer-subgroup.md) $H$ of one nonzero vector consequently has order $168/7=24$. There are three planes containing that vector, corresponding to the three lines of the two-dimensional quotient space. Adapted bases show $H$ acts transitively on these planes, so the [stabilizer](../../../../stabilizer-subgroup.md) of one such plane has order $24/3=8$.

Let $Q$ be any subgroup of order eight. Its [orbit](../../../../orbit-dynamical-system.md) lengths on the seven nonzero vectors are powers of two. Since their sum is odd, at least one [orbit](../../../../orbit-dynamical-system.md) has length one. Fix such a vector $v$. The action on the three planes through $v$ likewise has a fixed plane $P$. Thus $Q$ is contained in the [stabilizer](../../../../stabilizer-subgroup.md) of the [flag](../../../../flag-linear-algebra.md) $\langle v\rangle\subset P$, and equality follows because that [stabilizer](../../../../stabilizer-subgroup.md) already has order eight. The full [group](../../../../group-split.md) acts transitively on these flags, so all the subgroups are conjugate.

There are $7\cdot3=21$ flags. To see they yield distinct subgroups, use the standard upper unitriangular matrices relative to an adapted [basis](../../../../basis.md). Their only common nonzero fixed vector is the first [basis](../../../../basis.md) vector: varying entries in positions $(1,2)$ and $(1,3)$ forces the other two coordinates to vanish. On the quotient by that line, varying position $(2,3)$ leaves only the line of the second [basis](../../../../basis.md) vector fixed. Hence this subgroup fixes exactly one full [flag](../../../../flag-linear-algebra.md). Conjugation transfers uniqueness to each [flag](../../../../flag-linear-algebra.md) [stabilizer](../../../../stabilizer-subgroup.md), giving

$$
\boxed{21\text{ subgroups of order eight}}.
$$

## ↑ Ancestors (12)

1. [A2](../a2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
