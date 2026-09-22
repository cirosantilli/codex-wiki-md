<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

It is useful first to establish the global minimum, rather than only a stationary point. The [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md) $X=\Phi^\dagger\Phi$ has nonnegative [eigenvalues](../../../../../eigenvalue.md) $x_1,\ldots,x_N$. For fixed $r=\sum_i x_i$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\sum_i x_i^2\ge r^2/N$, with equality exactly when all $x_i$ are equal. Since $\alpha>0$,

$$
V\ge\frac12\left(\frac\alpha N+\beta\right)r^2+m^2r.
$$

For $m^2<0$ and $\beta>0$, this lower bound has its minimum at

$$
r=-\frac{Nm^2}{\alpha+N\beta},\qquad x_i=C^2=-\frac{m^2}{\alpha+N\beta}>0.
$$

The bound is attained, so every minimum has $\Phi^\dagger\Phi=C^2\mathbf1$, or $\Phi=CW$ with $W$ a [unitary matrix](../../../../../unitary-matrix.md). A global transformation removes $W$ by decomposing it into an overall phase and an $SU(N)$ matrix. Thus $\Phi_0=C\mathbf1$ is a valid representative of the [vacuum manifold](../../../../../vacuum-manifold.md).

Preservation of this chosen [vacuum expectation value](../../../../../vacuum-expectation-value.md) requires

$$
e^{i\theta}U_LU_R^\dagger=\mathbf1.
$$

Infinitesimally, with traceless Hermitian generators $L,R$, this reads $\theta\mathbf1+L-R=0$. Taking the [trace](../../../../../matrix-trace.md) forces $\theta=0$, and then $L=R$. The surviving continuous transformations are consequently

$$
\boxed{\Phi\mapsto U\Phi U^\dagger,\qquad U\in SU(N),\qquad H_{\mathrm{connected}}\simeq SU(N)_{\mathrm{diagonal}}.}
$$

All other independent continuous directions change the chosen [vacuum expectation value](../../../../../vacuum-expectation-value.md). Thus the number of broken generators is

$$
\boxed{[2(N^2-1)+1]-(N^2-1)=N^2.}
$$

Globally, taking the determinant of the stabilizer equation permits the discrete phases $e^{iN\theta}=1$, paired with $U_L=e^{-i\theta}U_R$. They induce the same conjugation action on $\Phi$. The faithful unbroken conjugation group is $SU(N)/\mathbb Z_N$; for example, at $N=2$, $U=-\mathbf1$ acts exactly like $U=\mathbf1$. Thus the question's description by $SU(N)$ is correct as a parametrization and at the [Lie algebra](../../../../../lie-algebra-split.md) level, with this central redundancy understood. It leaves the number of broken generators unchanged.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
