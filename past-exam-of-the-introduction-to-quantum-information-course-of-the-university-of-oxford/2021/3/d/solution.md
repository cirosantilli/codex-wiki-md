<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the unknown common eigenbasis as an unknown unit [Bloch vector](../../../../bloch-vector.md) $\mathbf n$. Then $\rho_A$ has vector $0.8\mathbf n$, while $\rho_B$ has vector $-0.4\mathbf n$. A single deterministic channel working for every possible basis must therefore map $0.8\mathbf n$ to $-0.4\mathbf n$ for every unit $\mathbf n$.

By the [basis-independent conversion of qubit Bloch radii](../../../../basis-independent-conversion-of-qubit-bloch-radii.md), linearity forces that channel to be $\mathcal E_{-1/2}$. Explicitly, add the conditions for $\mathbf n$ and $-\mathbf n$ to get $\mathcal E(I)=I$, then use the three coordinate directions to fix its action on every Pauli matrix. But $-1/2<-1/3$, so part [iv](../c/iv.md) excludes complete positivity. Thus **the forward conversion cannot be implemented reliably without knowing the basis**.

The reverse conversion would require $\mathcal E_{-2}$, which is not even positive by part [ii](../c/ii.md). Therefore **the reverse conversion is also impossible**. Unitary operations interspersed with physically allowed depolarizing maps cannot evade these restrictions: their composition remains a physical [quantum channel](../../../../quantum-channel.md). The question concerns one basis-independent operation on the supplied qubit, not an additional resource of many copies for learning its basis.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
