<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

Put $\boldsymbol\pi=\boldsymbol p-e\boldsymbol A/c=m\dot{\boldsymbol q}$. From [Hamilton's equations](../../../../../hamilton-s-equations.md),

$$
\dot q_i=\frac{\pi_i}{m},\qquad \dot p_i=\frac e{mc}\pi_j\partial_iA_j.
$$

For the stated time-independent [vector potential](../../../../../vector-potential.md), differentiating $\pi_i$ gives $m\ddot q_i=(e/c)\dot q_j(\partial_iA_j-\partial_jA_i)$, or

$$
\boxed{m\ddot{\boldsymbol q}=\frac ec\dot{\boldsymbol q}\times\boldsymbol B,\qquad\boldsymbol B=\nabla\times\boldsymbol A.}
$$

Use the [Poisson bracket](../../../../../poisson-bracket.md) convention $[F,G]=\sum_i(F_{q_i}G_{p_i}-F_{p_i}G_{q_i})$. Then direct differentiation gives

$$
\boxed{[\pi_i,q_j]=-\delta_{ij},\qquad[\pi_i,\pi_j]=\frac ec(\partial_iA_j-\partial_jA_i).}
$$

For $\boldsymbol A=(0,0,F(r))$ with $r=\sqrt{x_1^2+x_2^2}$, the Hamiltonian is independent of $x_3$, so $\dot p_3=0$. The radial force in the horizontal plane is $\dot p_r=e(p_3-eF/c)F'/(mc)$. For circular motion the radial acceleration is $-r\Omega^2$, and $p_r$ is the mechanical radial momentum because the horizontal [vector potential](../../../../../vector-potential.md) vanishes. Thus

$$
\boxed{\Omega^2=-\left(p_3-\frac{eF}{c}\right)\frac e{m^2cr}\frac{dF}{dr}.}
$$

A circular orbit at that radius is possible when the right side is nonnegative; positive values give either sense of horizontal rotation, and the longitudinal velocity is the constant $(p_3-eF(r)/c)/m$ along that orbit.

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
