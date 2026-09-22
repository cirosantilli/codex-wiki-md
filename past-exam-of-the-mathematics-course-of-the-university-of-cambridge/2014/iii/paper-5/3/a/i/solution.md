<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For this [Neumann Poisson problem](../../../../../../../neumann-poisson-problem.md), interpret the forcing in $L^2(U)$, as is automatic if it is [smooth](../../../../../../../smooth-function.md) up to the boundary. Literal interior smoothness alone does not ensure the integrals or bounded functionals required in this question: for example, $f(x)=x^{-2}$ on $(0,1)$ is interior [smooth](../../../../../../../smooth-function.md) but even $\int f\cdot1$ diverges. Classical regularity in the converse is likewise understood up to the boundary.

Suppose the [weak solution](../../../../../../../weak-solution.md) is [smooth](../../../../../../../smooth-function.md) on $\overline U$. Testing against compactly supported [test functions](../../../../../../../test-function.md) gives $-\Delta u=f$ in distributions and hence pointwise. Now the weak identity and [Green's first identity](../../../../../../../green-s-first-identity.md) imply

$$
0=\int_U\nabla u\cdot\nabla v-\int_Ufv=\int_{\partial U}(\partial_nu)v\,dS
$$

for every [smooth](../../../../../../../smooth-function.md) $v$ on $\overline U$. Every [smooth](../../../../../../../smooth-function.md) boundary function has such an extension, so $\partial_nu=0$ on $\partial U$. This proves both the interior equation and the boundary condition.

Conversely, for $u\in C^2(\overline U)$ satisfying the equation and zero [normal derivative](../../../../../../../normal-derivative.md), [Green's first identity](../../../../../../../green-s-first-identity.md) gives the weak identity for all [smooth](../../../../../../../smooth-function.md) $v$ on $\overline U$. The [density of smooth functions in a Sobolev space](../../../../../../../density-of-smooth-functions-in-a-sobolev-space.md) and the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) extend it continuously to every $v\in H^1(U)$. Thus **the classical solution is a [weak solution](../../../../../../../weak-solution.md)**, and the smooth [weak solution](../../../../../../../weak-solution.md) is classical.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
