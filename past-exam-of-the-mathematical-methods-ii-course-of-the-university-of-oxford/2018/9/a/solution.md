<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [divergence theorem](../../../../divergence-theorem.md) to $A(r)=(C\cdot r)(C'\cdot r)J(r)$. Since $C,C'$ are constant and $J$ is a [solenoidal vector field](../../../../solenoidal-vector-field.md), the [product rule](../../../../product-rule.md) gives

$$
\nabla\cdot A=(C\cdot J)(C'\cdot r)+(C'\cdot J)(C\cdot r).
$$

Its boundary flux vanishes when $J$ has [compact support](../../../../compact-support.md), or when its normal component vanishes on the boundary of the integration volume. Integrating therefore proves

$$
\boxed{\int_V(C\cdot r)(C'\cdot J)\,dV=-\int_V(C'\cdot r)(C\cdot J)\,dV.}
$$

For a discontinuous field, the divergence-free hypothesis must include its boundary jump, in the sense of a [weak derivative](../../../../weak-derivative.md). A field that merely has zero [divergence](../../../../divergence.md) at interior points can still have a nonzero surface source; that weaker hypothesis would not justify discarding the flux. The result is the [antisymmetric first moment of a localized solenoidal field](../../../../antisymmetric-first-moment-of-a-localized-solenoidal-field.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
