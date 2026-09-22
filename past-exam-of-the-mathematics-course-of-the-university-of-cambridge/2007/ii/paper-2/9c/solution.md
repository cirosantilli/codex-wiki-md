<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are

$$
\frac d{dt}\left(m\dot r_i+\frac ec A_i\right)=\frac ec\dot r_j\partial_iA_j.
$$

Using time [independence](../../../../../independent-random-variables.md) of the [vector potential](../../../../../vector-potential.md) gives $m\ddot r_i=(e/c)\dot r_j(\partial_iA_j-\partial_jA_i)$, which is the component form of

$$
\boxed{m\ddot{\mathbf r}=\frac ec\dot{\mathbf r}\times\mathbf B.}
$$

Taking its scalar product with the velocity shows $\dot T=m\dot{\mathbf r}\cdot\ddot{\mathbf r}=0$: **the [kinetic energy](../../../../../kinetic-energy.md) is constant**, since the magnetic force does no work.

For $\mathbf B=(0,0,F'(x))$, the equations give $m\ddot y=-(e/c)F'(x)\dot x$ and $\ddot z=0$. Thus $mc\dot y+eF(x)=-C$ and $\dot z=v_z$ are constants of motion. Substitution into $2T/m=\dot x^2+\dot y^2+\dot z^2$ yields

$$
\boxed{\dot x^2=\frac{2T}{m}-\frac{(eF(x)+C)^2}{m^2c^2}+D,\qquad D=-v_z^2.}
$$

The constant $D$ in this representation is nonpositive. The gauge choice $\mathbf A=(0,F(x),0)$ also makes the conserved transverse canonical momenta explicit.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
