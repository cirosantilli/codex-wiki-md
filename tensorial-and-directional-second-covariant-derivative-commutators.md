# Tensorial and directional second covariant derivative commutators

↑ **Parent:** [Commutator of covariant derivatives](commutator-of-covariant-derivatives.md)

For a [vector field](vector-field.md) $V$, the tensorial second derivative is $\nabla^2V(X,Y)=\nabla_X\nabla_YV-\nabla_{\nabla_XY}V$. With $R(X,Y)V=\nabla_X\nabla_YV-\nabla_Y\nabla_XV-\nabla_{[X,Y]}V$ and geometric [torsion tensor](torsion-tensor.md) $\mathcal T$, antisymmetrization gives

$$
\nabla^2V(X,Y)-\nabla^2V(Y,X)=R(X,Y)V-\nabla_{\mathcal T(X,Y)}V.
$$

This follows by subtracting the two definitions and using $\nabla_XY-\nabla_YX=[X,Y]+\mathcal T(X,Y)$. By contrast, the directional operator commutator subtracts no derivative-index connection and obeys $[\nabla_X,\nabla_Y]V=R(X,Y)V+\nabla_{[X,Y]}V$. On scalars the directional commutator is $[X,Y]f$, while the tensorial Hessian commutator is $-\mathcal T(X,Y)f$. Distinguishing these objects prevents an apparent contradiction when a scalar Hessian has an antisymmetric part despite commuting coordinate vector fields.

## ↑ Ancestors (6)

1. [Commutator of covariant derivatives](commutator-of-covariant-derivatives.md)
2. [Riemann curvature tensor](riemann-curvature-tensor-split.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
