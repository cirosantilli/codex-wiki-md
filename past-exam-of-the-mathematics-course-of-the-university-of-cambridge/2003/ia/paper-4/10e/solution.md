<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

For positive [masses](../../../../../mass.md) and distinct positions, [Newtonian gravitational field](../../../../../newtonian-gravitational-field.md) gives

$$
\boxed{m_i\ddot{\mathbf x}_i=-\sum_{j\ne i}\frac{Gm_im_j(\mathbf x_i-\mathbf x_j)}{|\mathbf x_i-\mathbf x_j|^3}}.
$$

Insert $\mathbf x_i=a(t)\mathbf a_i$ with $a>0$. The separation numerator contributes a factor $a$ and the denominator $a^3$, so

$$
m_i\ddot a\,\mathbf a_i=-\frac{\mathbf G_i}{a^2},\qquad \mathbf G_i=\sum_{j\ne i}\frac{Gm_im_j(\mathbf a_i-\mathbf a_j)}{|\mathbf a_i-\mathbf a_j|^3}.
$$

Hence the time-dependent equations are satisfied whenever

$$
\boxed{\mathbf G_i=\Lambda m_i\mathbf a_i\text{ for every }i,\qquad \ddot a=-\frac\Lambda{a^2}}.
$$

The fixed-shape condition is a [Newtonian central configuration](../../../../../newtonian-central-configuration.md), and the resulting motion is a [homothetic gravitational motion](../../../../../homothetic-gravitational-motion.md). It applies away from the collision scale $a=0$; a negative scale would require absolute values in the force scaling rather than the same positive-scale formula.

Multiplying the scalar equation by $\dot a$ gives

$$
\frac{d}{dt}\left(\frac{\dot a^2}{2}-\frac\Lambda a\right)=\dot a\left(\ddot a+\frac\Lambda{a^2}\right)=0.
$$

Thus its [first integral](../../../../../first-integral.md) is $\dot a^2/2-\Lambda/a=k/2$ for some real constant $k$.

In the pair potential

$$
W=-\sum_{j<i}\frac{Gm_im_j}{|\mathbf a_i-\mathbf a_j|},
$$

differentiating a pair with respect to $\mathbf a_i$ produces $Gm_im_j(\mathbf a_i-\mathbf a_j)/|\mathbf a_i-\mathbf a_j|^3$. Every pair incident on $i$ contributes exactly once, so $\nabla_iW=\mathbf G_i$. Moreover $W(\lambda\mathbf a_1,\ldots,\lambda\mathbf a_n)=\lambda^{-1}W$ for $\lambda>0$. Differentiating with respect to $\lambda$ at one proves the relevant [Euler homogeneous function theorem](../../../../../euler-theorem-for-homogeneous-functions.md) identity directly:

$$
\sum_i\mathbf a_i\cdot\mathbf G_i=-W.
$$

Dot each fixed-shape equation with $\mathbf a_i$ and sum to obtain

$$
\boxed{\Lambda I=-W,\qquad I=\sum_i m_i|\mathbf a_i|^2}.
$$

For a nontrivial collision-free configuration with at least two positive [masses](../../../../../mass.md), $W<0$ and $I>0$, and therefore $\Lambda>0$. Positivity requires an interacting pair; an isolated one-particle system is the degenerate zero-force exception rather than a positive-$\Lambda$ gravitational configuration. Pairwise cancellation also gives $\sum_i\mathbf G_i=0$, so the nondegenerate configuration has $\sum_i m_i\mathbf a_i=0$: its scaling origin is the [centre of mass](../../../../../center-of-mass.md).

Finally, the system's [kinetic energy](../../../../../kinetic-energy.md) is $I\dot a^2/2$ and its [potential energy](../../../../../potential-energy.md) is $W/a$. Consequently

$$
\boxed{E_{\rm total}=\frac I2\dot a^2+\frac Wa=I\left(\frac{\dot a^2}{2}-\frac\Lambda a\right)=\frac{kI}{2}}.
$$

This establishes the [energy](../../../../../energy.md) relation for every fixed configuration satisfying the algebraic condition, without assuming any particular particle arrangement.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
