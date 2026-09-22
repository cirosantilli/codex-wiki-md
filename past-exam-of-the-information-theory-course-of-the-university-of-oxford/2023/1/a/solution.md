<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The inequality is true** for ordinary addition, and also for addition in a [group](../../../../group-split.md). For any fixed $y$, the translation $x\mapsto x+y$ is [injective](../../../../injective-function.md), so it merely relabels the [probability masses](../../../../probability-mass.md) in the [conditional distribution](../../../../conditional-distribution.md). Since $X,Y$ are [independent random variables](../../../../independent-random-variables.md),

$$
H(X+Y\mid Y=y)=H(X\mid Y=y)=H(X).
$$

Averaging over $y$ and using [conditioning reduces entropy](../../../../conditioning-reduces-entropy.md) proves [entropy monotonicity under independent addition](../../../../entropy-monotonicity-under-independent-addition.md):

$$
\boxed{H(X+Y)\geq H(X+Y\mid Y)=H(X).}
$$

There is no requirement that $X+Y$ remain in the original [finite alphabet](../../../../finite-alphabet.md). The proof also gives $H(X+Y)\geq H(Y)$ by symmetry. Independence matters: for a nonconstant $X$ and $Y=-X$, the sum is constant while $H(X)>0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
