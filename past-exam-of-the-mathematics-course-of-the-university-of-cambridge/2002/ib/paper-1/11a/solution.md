<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

Put $\mu=\cos\vartheta$ and separate $\Phi=R(r)Y(\mu)$. Multiplying Laplace's equation by $r^2/(RY)$ gives

$$
\frac{(r^2R')'}R=-\frac{[(1-\mu^2)Y']'}Y=\lambda.
$$

For the regular [polynomial](../../../../../polynomial-split.md) angular modes, $\lambda=n(n+1)$ and $Y=P_n(\mu)$ is a [Legendre polynomial](../../../../../legendre-polynomial.md). The radial equation has branches $r^n$ and $r^{-n-1}$. Regularity at the origin keeps only the first inside, and decay at infinity keeps only the second outside. [Continuity](../../../../../continuous-function.md) at $r=1$ identifies their coefficients, so a mode has

$$
\Phi_n^{\rm in}=a_nr^nP_n(\mu),\qquad\Phi_n^{\rm out}=a_nr^{-n-1}P_n(\mu).
$$

Its outward-minus-inward radial derivative is $-(2n+1)a_nP_n(\mu)$. The prescribed angular dependence decomposes as $V\mu^2=VP_0/3+2VP_2/3$, since $P_0=1$ and $P_2=(3\mu^2-1)/2$. Hence $a_0=-V/3$ and $a_2=-2V/15$, with no other required modes. The [spherical harmonic matching with a derivative jump](../../../../../spherical-harmonic-matching-with-a-derivative-jump.md) gives

$$
\boxed{\Phi(r,\vartheta)=\begin{cases}-\dfrac V3-\dfrac{2V}{15}r^2P_2(\cos\vartheta),&r<1,\\-\dfrac{V}{3r}-\dfrac{2V}{15r^3}P_2(\cos\vartheta),&r>1.\end{cases}}
$$

Both branches are harmonic in their respective regions. They agree at the sphere, and their derivative jump is $V/3+(2V/3)P_2=V\cos^2\vartheta$. The interior is regular at zero and the exterior decays at infinity. An additional homogeneous matching mode would satisfy $-(2n+1)a_n=0$, so its coefficient vanishes.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
