<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a bounded [volume](../../../../volume.md) $V$ with outward-oriented piecewise smooth boundary $S$, the [divergence theorem](../../../../divergence-theorem.md) states

$$
\boxed{\iint_SG\cdot n\,dS=\iiint_V\nabla\cdot G\,dV.}
$$

Here $G$ is a continuously differentiable [vector field](../../../../vector-field.md) on a neighborhood of $V$, $n$ the outward unit [normal vector](../../../../normal-vector.md), and $dV$ the [volume element](../../../../volume-element.md). The left side is its outward [flux](../../../../flux.md).

For a twice continuously differentiable field $F$, equality of mixed [partial derivatives](../../../../partial-derivative.md) gives

$$
\nabla\cdot(\nabla\times F)
=(F_{z,yx}-F_{y,zx})+(F_{x,zy}-F_{z,xy})+(F_{y,xz}-F_{x,yz})=0.
$$

Apply the [divergence theorem](../../../../divergence-theorem.md) to $G=\nabla\times F$ to obtain

$$
\boxed{\iint_S(\nabla\times F)\cdot d\boldsymbol S=0.}
$$

The regularity hypotheses justify differentiating and integrating the [curl](../../../../curl.md); a field singularity cannot simply be ignored in a volume argument.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
