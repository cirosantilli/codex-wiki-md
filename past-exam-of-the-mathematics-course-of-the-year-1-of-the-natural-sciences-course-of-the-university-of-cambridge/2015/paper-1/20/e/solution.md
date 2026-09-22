<h1 id="20/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For an oriented surface $S'$ with compatible boundary direction, the [Stokes theorem](../../../../../stokes-theorem.md) states

$$
\boxed{\oint_{\partial S'}\mathbf v\cdot d\mathbf r
=\int_{S'}(\boldsymbol\nabla\times\mathbf v)\cdot\mathbf n\,dS.}
$$

Let $H$ denote the removed patch and $S'=S\setminus H$ the remaining cylinder. Keep the outward orientation inherited from the closed cylinder. Everywhere on the removed curved patch, the normal [curl](../../../../../curl.md) component is $-\alpha R$, so its [flux](../../../../../flux.md) is $-\alpha RA$, where $A$ is its actual curved area. Part (d) then gives

$$
\int_{S'}(\boldsymbol\nabla\times\mathbf v)\cdot\mathbf n\,dS
=0-(-\alpha RA)=\alpha RA.
$$

Consequently the [circulation around a hole in an oriented surface](../../../../../circulation-around-a-hole-in-an-oriented-surface.md) is

$$
\boxed{\oint_{\partial S'}\mathbf v\cdot d\mathbf r=\alpha RA.}
$$

The positive direction here is induced by the **remaining** outward-oriented surface; locally it runs clockwise around the hole when viewed from outside. If the edge is instead traversed positively around the **removed** patch, the direction reverses and the answer is **$-\alpha RA$**. The question does not specify an edge direction, so the sign must be accompanied by this convention. The result depends only on the removed curved area, not on its shape. If the patch has several boundary components, use the sum of their induced [line integrals](../../../../../line-integral.md). Since $[\alpha]=1/(\text{length}\cdot\text{time})$, the result has the units of a [velocity](../../../../../velocity.md) [line integral](../../../../../line-integral.md), length squared per time.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
