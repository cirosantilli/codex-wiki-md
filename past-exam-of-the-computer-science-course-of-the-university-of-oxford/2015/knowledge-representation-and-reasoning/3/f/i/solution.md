<h1 id="3/f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For polynomial-time many-one reductions, an unconditional example is the [empty language](../../../../../../empty-language.md):

$$
\boxed{L=\varnothing\text{ is in NP and is not NP-complete}.}
$$

A procedure that rejects every input decides it in constant time, so it belongs to [P](../../../../../../p-complexity.md) and hence [NP](../../../../../../np-complexity.md). It is not [NP-hard](../../../../../../np-hardness.md): the nonempty [formal language](../../../../../../formal-language.md) $\{0\}$ belongs to [NP](../../../../../../np-complexity.md), but no many-one reduction $f$ can satisfy

$$
0\in\{0\}\quad\Longleftrightarrow\quad f(0)\in\varnothing.
$$

The right-hand side is always false. Thus the hardness condition fails without assuming $\mathsf P\ne\mathsf{NP}$. Giving an ordinary nontrivial problem in [P](../../../../../../p-complexity.md) would not establish the requested separation unconditionally, because that would require excluding the possibility $\mathsf P=\mathsf{NP}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [F](../../f.md)
3. [3](../../../3.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
