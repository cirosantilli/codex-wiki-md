<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

Apply the rotating-vector derivative rule first to the position [vector](../../../../../vector.md) and then to its [velocity](../../../../../velocity.md). Since $\boldsymbol\omega$ is constant,

$$
\mathbf v=\mathbf v'+\boldsymbol\omega\times\mathbf x,\qquad \mathbf a=\mathbf a'+2\boldsymbol\omega\times\mathbf v'+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x).
$$

For example, the derivative of $\mathbf v'$ contributes $\mathbf a'+\boldsymbol\omega\times\mathbf v'$, while that of $\boldsymbol\omega\times\mathbf x$ contributes the other two terms. This is the [equation of motion in a rotating frame](../../../../../equation-of-motion-in-a-rotating-frame.md). The mutual [central forces](../../../../../central-force.md) are unchanged in form because rotations preserve lengths and differences of position vectors. [Newton's second law](../../../../../newton-s-second-law.md) for particle $i$ becomes

$$
m\mathbf a_i'=\sum_{j\ne i}\mathbf F_{ij}+e(\mathbf v_i'+\boldsymbol\omega\times\mathbf x_i)\times\mathbf B-2m\boldsymbol\omega\times\mathbf v_i'-m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x_i).
$$

Set $\boldsymbol\omega=-e\mathbf B/(2m)$. The velocity-dependent [Lorentz force](../../../../../lorentz-force.md) is $e\mathbf v_i'\times\mathbf B=-e\mathbf B\times\mathbf v_i'$, and it cancels the [Coriolis force](../../../../../coriolis-force.md) $-2m\boldsymbol\omega\times\mathbf v_i'=e\mathbf B\times\mathbf v_i'$. The remaining terms combine to $m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x_i)$ and are quadratic in the [magnetic field](../../../../../magnetic-field.md). Neglecting them gives

$$
\boxed{m\mathbf a_i'=\sum_{j\ne i}\mathbf F_{ij}+O(B^2)},
$$

identical to the zero-field equations to first order. The [Larmor theorem](../../../../../larmor-theorem.md) requires the common charge-to-mass ratio; a mixture with different ratios cannot use one rotating frame to cancel every magnetic term.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
