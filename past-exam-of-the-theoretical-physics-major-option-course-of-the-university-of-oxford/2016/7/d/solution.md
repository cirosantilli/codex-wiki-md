<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a Hermitian [gauge field](../../../../gauge-field.md) $A_\mu=A_\mu^AT^A$ and $\operatorname{tr}(T^AT^B)=\delta^{AB}/2$. With fundamental [covariant derivative](../../../../covariant-derivative.md) $\partial_\mu-igA_\mu$, the adjoint derivative is

$$
\boxed{D_\mu\Phi=\partial_\mu\Phi-ig[A_\mu,\Phi].}
$$

It transforms as $D_\mu\Phi\mapsto U(D_\mu\Phi)U^\dagger$, provided $A'_\mu=UA_\mu U^\dagger-(i/g)(\partial_\mu U)U^\dagger$.

The infinitesimal parameter in $U=1+i\epsilon+O(\epsilon^2)$ must be **Hermitian and traceless**, from unitarity and unit determinant. It is not generally antisymmetric as the hint states. The valid generator $\epsilon=\operatorname{diag}(1,-1,0,0,0)$ is a concrete counterexample to that assertion.

Choose canonical adjoint kinetic normalization $\mathcal L_\Phi=\operatorname{tr}(D_\mu\Phi D^\mu\Phi)$, which gives $\tfrac12\partial\Phi^A\partial\Phi^A$. For the diagonal [vacuum expectation value](../../../../vacuum-expectation-value.md) $D=v\operatorname{diag}(2,2,2,-3,-3)$, the matrix unit $E_{ij}$ obeys $[D,E_{ij}]=(d_i-d_j)E_{ij}$. Thus the [mass](../../../../mass.md) of the [gauge boson](../../../../gauge-boson.md) associated with either normalized Hermitian generator joining $i,j$ is $g|d_i-d_j|$.

Within the three-dimensional and two-dimensional blocks, or for diagonal generators, the commutator vanishes. There are therefore $8+3+1=12$ massless [gauge bosons](../../../../gauge-boson.md). The $3\times2$ interblock pairs supply two real generators each, hence 12 equally massive [gauge bosons](../../../../gauge-boson.md):

$$
\boxed{m_X=m_Y=5g|v|,\qquad
SU(5)\longrightarrow S(U(3)\times U(2))
\simeq\frac{SU(3)\times SU(2)\times U(1)}{\mathbb Z_6}.}
$$

The absolute mass formula assumes the stated kinetic normalization, which the question leaves implicit. Writing instead $\tfrac12\operatorname{tr}(D\Phi)^2$ without rescaling $\Phi$ would multiply these squared masses by $1/2$.

This is the gauge group of the [Standard Model](../../../../standard-model-split.md), up to its global quotient, arising from one adjoint [Higgs mechanism](../../../../higgs-mechanism.md) in a simple unified group. The unbroken abelian generator can be chosen as $Y=\operatorname{diag}(-1/3,-1/3,-1/3,1/2,1/2)$, so $D=-6vY$. This is the characteristic first breaking step of an [SU(5) grand unified theory](../../../../su-5-grand-unified-theory.md), rather than electroweak breaking all the way to electromagnetism.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
