<h1 id="k/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [streamline](../../../../streamline.md) is a curve whose tangent is parallel to the instantaneous fluid [velocity field](../../../../velocity-field.md). In steady flow one may parametrize it by $d\mathbf r/ds=\mathbf u(\mathbf r)$. Dotting the steady [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md) with $\mathbf u$ eliminates the cross-product term, since $\mathbf u\cdot((\nabla\times\mathbf u)\times\mathbf u)=0$. Hence

$$
\boxed{\mathbf u\cdot\nabla\left(p+\tfrac12\rho|\mathbf u|^2\right)=0,}
$$

which is [Bernoulli's principle](../../../../bernoulli-s-principle.md) along each streamline.

For the supplied field, $xu+yv=0$, so along a streamline

$$
\frac{d}{ds}(x^2+y^2)=2xu+2yv=0.
$$

Writing $r^2=x^2+y^2$, the tangential speed is $v_\theta=-br+c/r$ and the radial speed is zero. Both $r$ and $|\mathbf u|^2=(-br+c/r)^2$ are constant around each nonstagnant circular streamline. The Bernoulli quantity is constant there, so **the pressure is constant on every such circle**.

If a circle is wholly stagnant, the same conclusion follows directly from the steady [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md): on it $\mathbf u=0$ and $\nabla|\mathbf u|^2=0$, hence $\nabla p=0$. Equivalently the radial momentum equation gives $\nabla p=\rho(-br+c/r)^2\mathbf e_r/r$ and no angular pressure variation, including at zero tangential speed. Thus **$p$ is constant on $x^2+y^2=a^2$ for every nonzero $a$**, with no exception for a stagnation circle.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [K](../../k.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
