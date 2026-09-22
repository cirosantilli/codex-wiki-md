<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a binary hypothesis class $\mathcal H=\{x\mapsto f(x,\alpha)\}$, a set of $m$ distinct points is shattered if every one of its $2^m$ binary labelings is realized by some member of $\mathcal H$. The [VC dimension](../../../../../../vc-dimension.md) is

$$
\boxed{\operatorname{VC}(\mathcal H)=\sup\{m:\text{some }m\text{-point set is shattered by }\mathcal H\},}
$$

with value infinity if arbitrarily large finite sets are shattered. For real-valued scores, apply this definition to the associated binary decision functions, for example their signs. The word “some” matters: shattering every set of that size is not required.

As an example, take the interval classifiers on the real line, $f_{a,b}(x)=\mathbf1_{\{a\le x\le b\}}$. Two ordered points $x_1<x_2$ can receive labels $00$, $10$, $01$ or $11$ by choosing an interval away from both, around the first, around the second, or containing both. Hence the class shatters two points. No three ordered points can be shattered, since any interval containing the first and third also contains the middle, making labeling $101$ impossible. Thus the [VC dimension of interval indicators](../../../../../../vc-dimension-of-interval-indicators.md) is

$$
\boxed{\operatorname{VC}(\mathcal H)=2.}
$$

This describes combinatorial classification capacity, rather than merely counting written parameters; the definition applies equally to nonlinear or infinite-parameter classes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
