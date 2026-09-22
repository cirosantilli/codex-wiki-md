<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Green identity.** With $n$ the outward unit normal, the [product rule](../../../../product-rule.md) gives $\nabla\cdot(u\nabla v)=u\nabla^2v+\nabla u\cdot\nabla v$. Integrating over $V$ and applying the [divergence theorem](../../../../divergence-theorem.md) yields [Green's first identity](../../../../green-s-first-identity.md):

$$
\boxed{\int_V(u\nabla^2v+\nabla u\cdot\nabla v)\,dV=\int_Su\partial_nv\,dS.}
$$

**Uniqueness for nonzero mass.** Suppose two real solutions have the same prescribed boundary data, and let $w$ be their difference. The spatial equation called the [Klein-Gordon equation](../../../../klein-gordon-equation.md) in the question is the [modified Helmholtz equation](../../../../modified-helmholtz-equation.md), so $\nabla^2w=m^2w$. With $u=v=w$, [Green's first identity](../../../../green-s-first-identity.md) becomes

$$
\int_V(|\nabla w|^2+m^2w^2)\,dV=\int_Sw\partial_nw\,dS.
$$

For identical [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), $w=0$ on $S$; for identical [Neumann boundary conditions](../../../../neumann-boundary-condition.md), $\partial_nw=0$ there. Either makes the right-hand side zero. When $m$ is real and nonzero, both integrands on the left are nonnegative, forcing $w=0$. Thus

$$
\boxed{\text{For }m\ne0,\text{ either type of boundary data determines at most one solution.}}
$$

This is the required uniqueness assertion; existence is understood for admissible smooth data on a suitable bounded region. Complex-valued solutions obey the same result by treating their real and imaginary parts separately.

**Zero mass.** For $m=0$, the argument gives $\nabla w=0$, hence $w=C$ on the connected region. [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) still force $C=0$, but [Neumann boundary conditions](../../../../neumann-boundary-condition.md) leave an arbitrary additive constant:

$$
\boxed{m=0:\quad\text{Dirichlet uniqueness; Neumann uniqueness only up to a constant.}}
$$

The prescribed normal data in the zero-mass case must also satisfy $\int_S\partial_n\Phi\,dS=0$, by the [divergence theorem](../../../../divergence-theorem.md). For nonzero $m$, that flux can instead equal $m^2\int_V\Phi\,dV$.

**Energy minimization.** Let $\eta=w-v$ for the two functions in the last part. They share their boundary values, so $\eta=0$ on $S$. Since $v$ is a [harmonic function](../../../../harmonic-function.md), [Green's first identity](../../../../green-s-first-identity.md) gives

$$
\int_V\nabla v\cdot\nabla\eta\,dV=\int_S\eta\partial_nv\,dS-\int_V\eta\nabla^2v\,dV=0.
$$

Expand the square in the [Dirichlet energy](../../../../dirichlet-energy.md) of $w=v+\eta$:

$$
\int_V|\nabla w|^2\,dV=\int_V|\nabla v|^2\,dV+2\int_V\nabla v\cdot\nabla\eta\,dV+\int_V|\nabla\eta|^2\,dV.
$$

The cross term vanishes, so

$$
\boxed{\int_V|\nabla w|^2\,dV-\int_V|\nabla v|^2\,dV=\int_V|\nabla(w-v)|^2\,dV\geq0.}
$$

Equality requires $w-v$ to be constant, and the shared boundary values then make it zero. This is the [Dirichlet principle](../../../../dirichlet-principle.md): among functions with fixed boundary values, the [harmonic function](../../../../harmonic-function.md) minimizes [Dirichlet energy](../../../../dirichlet-energy.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
