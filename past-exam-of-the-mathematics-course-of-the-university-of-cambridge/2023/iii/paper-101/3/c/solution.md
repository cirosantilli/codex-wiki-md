<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An $A$-module $M$ is a [flat module](../../../../../../flat-module.md) when the [tensor functor](../../../../../../tensor-product-of-modules.md) $-\otimes_AM$ preserves injections, equivalently when it is exact.

Suppose first that $M$ is flat. For any nonzero $a\in A$, tensor the injection $A\xrightarrow{a}A$ with $M$. The resulting map $M\xrightarrow{a}M$ is injective, so $am=0$ implies $m=0$. Thus $M$ is a [torsion-free module](../../../../../../torsion-free-module.md).

Conversely, suppose $M$ is torsion-free over the [principal ideal domain](../../../../../../principal-ideal-domain.md) $A$. Every finitely generated submodule of $M$ is a finitely generated torsion-free module over a PID, hence a [finite free module](../../../../../../finite-free-module.md) and therefore flat. The module $M$ is the [filtered colimit](../../../../../../filtered-colimit-of-modules.md) of these submodules. Tensor products commute with filtered colimits, and filtered colimits of modules preserve exact sequences, so $M$ is flat. This proves that a [torsion-free module over a principal ideal domain is flat](../../../../../../torsion-free-module-over-a-principal-ideal-domain-is-flat.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
