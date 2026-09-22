<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A function on the open set $D$ is [holomorphic](../../../holomorphic-function-split.md) if at every $a\in D$ the complex limit

$$
f'(a)=\lim_{\substack{z\to a\\z\neq a}}
\frac{f(z)-f(a)}{z-a}
$$

exists. The limit is independent of the direction of approach.

A [pole](../../../pole.md) of order $n\geq1$ at $a$ means that $f(z)=(z-a)^{-n}h(z)$ in a punctured neighborhood, where $h$ extends holomorphically across $a$ and $h(a)\neq0$. Equivalently $(z-a)^nf(z)$ has a nonzero finite limit at $a$.

For the given quotient, $\cos z=1$ is equivalent, on putting $q=e^{iz}$, to $q+q^{-1}=2$, or $(q-1)^2=0$. Thus all possible [poles](../../../pole.md) are $a=2\pi k$, $k\in\mathbb Z$, with no additional nonreal solutions. At such a point,

$$
\cos z-1=-\tfrac12(z-a)^2+O((z-a)^4).
$$

At $a\neq0$ the numerator does not vanish, so the [pole](../../../pole.md) has order two. At zero the numerator cancels one order:

$$
\frac z{\cos z-1}=-\frac2z-\frac z6+O(z^3).
$$

Therefore

$$
\boxed{z=0\text{ is a simple pole};\quad
z=2\pi k,\ k\neq0,\text{ are double poles}.}
$$

The numerator's cancellation at zero is why not every denominator zero produces the same [pole](../../../pole.md) order.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
