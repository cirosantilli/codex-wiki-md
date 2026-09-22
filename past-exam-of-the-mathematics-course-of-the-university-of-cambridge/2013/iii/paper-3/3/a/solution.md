<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [symplectic group](../../../../../../symplectic-group.md) consists of the invertible linear maps preserving the [alternating bilinear form](../../../../../../alternating-bilinear-form.md):

$$
\operatorname{Sp}(V)=\{g\in\operatorname{GL}(V):(vg,wg)=(v,w)\text{ for all }v,w\in V\}.
$$

We use row-vector action in this question, which is the convention compatible with its printed upper-triangular flag [stabilizer subgroup](../../../../../../stabilizer-subgroup.md). Thus matrices preserve a form matrix $J$ by $gJg^T=J$.

Count ordered [symplectic bases](../../../../../../symplectic-basis.md). There are $q^{2m}-1$ choices for the first nonzero vector $e_1$. Nondegeneracy makes the equation $(e_1,f_1)=1$ a nonzero linear-functional equation, with $q^{2m-1}$ solutions. Their span is a nondegenerate plane; its [orthogonal complement](../../../../../../orthogonal-complement.md) is symplectic of dimension $2m-2$. Repeating there gives

$$
\boxed{|\operatorname{Sp}_{2m}(q)|=
\prod_{i=1}^m q^{2i-1}(q^{2i}-1)=q^{m^2}\prod_{i=1}^m(q^{2i}-1).}
$$

Each [symplectic basis](../../../../../../symplectic-basis.md) is the image of a fixed one under exactly one form-preserving map, justifying the count as a group order. If $q=p^a$, every factor $q^{2i}-1$ is prime to $p$, so the exact $p$-part is $q^{m^2}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
