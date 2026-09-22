<h1 id="14c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fixed-point conditions are

$$
0=N(1-S)-\beta IS,
\qquad
0=I\{(\beta-1)S-I\}.
$$

On $I=0$ they give $(S,I)=(0,0)$ and the [disease-free equilibrium](../../../../../../disease-free-equilibrium.md) $(1,0)$. An interior fixed point requires $I=(\beta-1)S$, so it exists only for $\beta>1$; substitution in the first equation gives the [endemic equilibrium](../../../../../../endemic-equilibrium.md)

$$
\boxed{(S_*,I_*)=\left(\frac1\beta,1-\frac1\beta\right).}
$$

The [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J(S,I)=
\begin{pmatrix}
1-2S-(1+\beta)I&1-(1+\beta)S\\
(\beta-1)I&(\beta-1)S-2I
\end{pmatrix}.
$$

At $(1,0)$ its eigenvalues are $-1$ and $\beta-1$. Hence $(1,0)$ is asymptotically stable for $\beta<1$ and a [saddle point](../../../../../../saddle-point.md) for $\beta>1$. At the endemic equilibrium, the equivalent $(N,\theta)$ coordinates give eigenvalues $-1$ and $1-\beta$, so it is a stable node whenever it exists. The origin is unstable because every solution with $N(0)>0$ has $N(t)\to1$.

For the [phase portrait](../../../../../../phase-portrait.md), the line $I=0$ is invariant and points toward $(1,0)$. Also

$$
\dot I=I\{(\beta-1)S-I\},
\qquad
\dot N=N(1-N),
$$

so trajectories move toward the line $S+I=1$. If $\beta<1$, then $\dot I<0$ throughout the interior and every nonzero solution approaches $(1,0)$. If $\beta>1$, the additional infective nullcline is the ray $I=(\beta-1)S$; $I$ increases below this ray and decreases above it, and every trajectory with $I(0)>0$ approaches $(1/\beta,1-1/\beta)$. At $\beta=1$ the disease-free and endemic branches exchange stability in a [transcritical bifurcation](../../../../../../transcritical-bifurcation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14C](../../14c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
