# Energy uniqueness for a linear elastic traction problem

↑ **Parent:** [Linear elasticity](linear-elasticity.md)

On a connected isotropic [linear elastic](linear-elasticity.md) body, assume $\mu>0$ and $3\lambda+2\mu>0$. Then $W(e)=\mu|e^{\rm dev}|^2+(3\lambda+2\mu)(\operatorname{tr}e)^2/6$ is positive for every nonzero symmetric [strain tensor](infinitesimal-strain-tensor.md). If two equilibria have the same [body force](body-force.md) and boundary [traction](traction.md), their difference $v$ satisfies zero loading. Multiplication of equilibrium by $v$ and the [divergence theorem](divergence-theorem.md) yield $\int_B2W(e(v))\,dV=0$. Hence $e(v)=0$, and the kernel of the symmetric gradient consists of infinitesimal translations and rotations: $v=a+\omega\times x$.

The conclusion is uniqueness modulo these modes, not existence for arbitrary tractions. Existence additionally requires zero total resultant force and torque. On a disconnected body each connected component has its own rigid modes; fixing enough displacements removes those modes and can produce full uniqueness.

## ↑ Ancestors (6)

1. [Linear elasticity](linear-elasticity.md)
2. [Elasticity (physics)](elasticity-physics-split.md)
3. [Continuum mechanics](continuum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-elasticity-and-plasticity-course-of-the-university-of-oxford/2008/1/d/solution.md)
