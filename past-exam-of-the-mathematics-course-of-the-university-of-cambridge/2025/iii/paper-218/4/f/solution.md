<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The assignment `nn.model.i <- nn.model` does not construct a fresh untrained Keras model: it aliases an object whose weights were already fitted using every training observation, including the nominally held-out one, and repeated fits continue mutating those weights. This [data leakage](../../../../../../data-leakage.md) makes metric2 severely optimistic. Moreover, random leave-one-out validation among reviews from 2012--2025 does not reproduce the [dataset shift](../../../../../../dataset-shift.md) to new recent reviews that metric1 measures.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
