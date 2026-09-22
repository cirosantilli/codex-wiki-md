<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

For distinct positions and positive masses, [Newton's law of universal gravitation](../../../../../newton-s-law-of-universal-gravitation.md) gives

$$
m_i\ddot{\mathbf x}_i=-G\sum_{j\ne i}m_im_j\frac{\mathbf x_i-\mathbf x_j}{|\mathbf x_i-\mathbf x_j|^3}.
$$

The proposed [homothetic gravitational motion](../../../../../homothetic-gravitational-motion.md) has $\ddot{\mathbf x}_i=-(2/9)t^{-4/3}\mathbf a_i$ and pair distances $t^{2/3}|\mathbf a_i-\mathbf a_j|$, so cancellation of $t^{-4/3}$ gives the time-independent equations

$$
\boxed{\frac29\mathbf a_i=G\sum_{j\ne i}m_j\frac{\mathbf a_i-\mathbf a_j}{|\mathbf a_i-\mathbf a_j|^3}}.
$$

These define a [Newtonian central configuration](../../../../../newtonian-central-configuration.md) with this choice of scale. For

$$
\Phi=\frac19\sum_i m_i|\mathbf a_i|^2+\sum_{i<j}\frac{Gm_im_j}{|\mathbf a_i-\mathbf a_j|},
$$

[differentiation](../../../../../differentiation.md) in $\mathbf a_i$ gives $\nabla_{\mathbf a_i}\Phi=(2/9)m_i\mathbf a_i-G\sum_{j\ne i}m_im_j(\mathbf a_i-\mathbf a_j)/|\mathbf a_i-\mathbf a_j|^3=0$, exactly the displayed equations. The double sum in the paper counts each pair twice, so it agrees with this expression.

Multiply the configuration equations by $m_i$ and sum. Pair contributions cancel, giving $\sum_i m_i\mathbf a_i=0$. Thus the total [linear momentum](../../../../../momentum.md) is $\mathbf P=(2/3)t^{-1/3}\sum_i m_i\mathbf a_i=0$. Each position is parallel to its [velocity](../../../../../velocity.md), so every $m_i\mathbf x_i\times\dot{\mathbf x}_i=0$ and the total [angular momentum](../../../../../angular-momentum.md) is zero. About any other fixed point $\mathbf b$, it is $\mathbf L_{\mathbf b}=\mathbf L_O-\mathbf b\times\mathbf P=\boxed{\mathbf0}$.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
