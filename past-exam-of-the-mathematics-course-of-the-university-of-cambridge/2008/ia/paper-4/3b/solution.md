<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

Put $M=m_1+m_2$ and let $\mathbf R=(m_1\mathbf r_1+m_2\mathbf r_2)/M$ be the [center of mass](../../../../../center-of-mass.md). Applying [Newton's second law](../../../../../newton-s-second-law.md) separately to the two [point masses](../../../../../point-mass.md) gives

$$
m_1\ddot{\mathbf r}_1=\mathbf f,\qquad m_2\ddot{\mathbf r}_2=-\mathbf f,\qquad M\ddot{\mathbf R}=0.
$$

Thus the [center of mass](../../../../../center-of-mass.md) has constant [velocity](../../../../../velocity.md), $\mathbf R(t)=\mathbf R(0)+t\dot{\mathbf R}(0)$. For the relative [position](../../../../../position.md) $\mathbf r=\mathbf r_1-\mathbf r_2$, subtraction gives

$$
\ddot{\mathbf r}=\left(\frac1{m_1}+\frac1{m_2}\right)\mathbf f,\qquad \boxed{\mu\ddot{\mathbf r}=\mathbf f},\qquad \mu=\frac{m_1m_2}{m_1+m_2}.
$$

Here $\mu$ is the [reduced mass](../../../../../reduced-mass.md); it converts the relative motion into a one-body [equation of motion](../../../../../equation-of-motion.md).

For the given linear [force](../../../../../force.md), the relative [position](../../../../../position.md) obeys [simple harmonic motion](../../../../../simple-harmonic-motion.md), $\ddot{\mathbf r}+\Omega^2\mathbf r=0$, where $\Omega^2=k/\mu$. The initial rest condition gives

$$
\mathbf r(t)=\mathbf r(0)\cos(\Omega t),\qquad |\mathbf r(0)|=d.
$$

For $d>0$, collision first occurs when the relative [position](../../../../../position.md) vanishes, namely when $\Omega t=\pi/2$. Therefore

$$
\boxed{t_{\rm collision}=\frac\pi2\sqrt{\frac{m_1m_2}{k(m_1+m_2)}}}.
$$

The separation $d$ cancels because the [frequency](../../../../../frequency.md) of this [simple harmonic motion](../../../../../simple-harmonic-motion.md) is independent of its [amplitude](../../../../../wave-amplitude.md).

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
