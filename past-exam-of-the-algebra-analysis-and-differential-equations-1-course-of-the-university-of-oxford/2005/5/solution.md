<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [pole](../../../pole.md) of order $m$ at $a$ means that $f(z)=h(z)/(z-a)^m$ near $a$, where $h$ is holomorphic and $h(a)\ne0$. Equivalently its [Laurent series](../../../laurent-series.md) has a finite principal part with leading nonzero term $a_{-m}(z-a)^{-m}$. The [residue](../../../residue.md) $c$ is the coefficient $a_{-1}$. For a simple pole, $m=1$, this coefficient is $h(a)$, so

$$
\boxed{\operatorname{Res}_{z=a}f=\lim_{z\to a}(z-a)f(z).}
$$

For $\cot z=\cos z/\sin z$, the zeros of the denominator are exactly $z=n\pi$, $n\in\mathbb Z$: this follows from $e^{2iz}=1$. Each is simple, because $\sin'(n\pi)=\cos(n\pi)=(-1)^n\ne0$. Therefore

$$
\boxed{\cot z\text{ has simple poles at }n\pi,\quad\operatorname{Res}_{z=n\pi}\cot z=1.}
$$

There are no other finite [singularities](../../../complex-singularity.md). If infinity is included, it is an accumulation point of these poles, so it is not an isolated singularity to which the usual removable/pole/essential classification could be applied.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2005](../../2005-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
