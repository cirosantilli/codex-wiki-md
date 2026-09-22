<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Introduce $\mathbf e_i=(\cos\theta_i,\sin\theta_i)$ and $\mathbf e_i^\perp=(-\sin\theta_i,\cos\theta_i)$. The joint and tip positions are

$$
\mathbf r_A=\ell\mathbf e_1,
\qquad
\mathbf r_B=\ell(\mathbf e_1+\mathbf e_2),
$$

so

$$
\dot{\mathbf r}_A=\ell\dot\theta_1\mathbf e_1^\perp,
\qquad
\dot{\mathbf r}_B=\ell(\dot\theta_1\mathbf e_1^\perp
+\dot\theta_2\mathbf e_2^\perp).
$$

Using the point drags $\mathbf F_A=-\zeta\dot{\mathbf r}_A$, $\mathbf F_B=-\zeta\dot{\mathbf r}_B$, and the follower force $\boldsymbol\Gamma=-\Gamma\mathbf e_2$ in the [principle of virtual work](../../../../../virtual-work.md) gives the independent coefficients of $\delta\theta_1$ and $\delta\theta_2$:

$$
\begin{aligned}
\zeta\ell^2[2\dot\theta_1+\cos(\theta_1-\theta_2)\dot\theta_2]
+2k\theta_1-k\theta_2-\Gamma\ell\sin(\theta_1-\theta_2)&=0,\\
\zeta\ell^2[\dot\theta_2+\cos(\theta_1-\theta_2)\dot\theta_1]
-k\theta_1+k\theta_2&=0.
\end{aligned}
$$

With scaled time $s=kt/(\zeta\ell^2)$ and [dimensionless follower load](../../../../../dimensionless-follower-load.md) $\Sigma=\Gamma\ell/k$, these are exactly the stated equations with primes denoting $d/ds$.

If the two links are constrained to remain collinear, their admissible virtual rotations satisfy $\delta\theta_1=\delta\theta_2$. Adding the two generalized equations and putting $\theta_1=\theta_2=\theta$ gives

$$
\boxed{5\theta'+\theta=0,
\qquad \theta(s)=\theta(0)e^{-s/5}.}
$$

The drag factor five is the sum of the squared lever arms $1^2+2^2$. The follower force lies along the straight filament and has no moment, so it cannot affect this rigid rotational relaxation.

For unrestricted perturbations, linearization about the straight state gives

$$
\begin{pmatrix}2&1\\1&1\end{pmatrix}
\begin{pmatrix}\theta_1'\\\theta_2'\end{pmatrix}
+
\begin{pmatrix}2-\Sigma&\Sigma-1\\-1&1\end{pmatrix}
\begin{pmatrix}\theta_1\\\theta_2\end{pmatrix}=0.
$$

For modes proportional to $e^{\lambda s}$,

$$
\lambda^2+(6-2\Sigma)\lambda+1=0,
$$

and therefore

$$
\boxed{\lambda_\pm=\Sigma-3
\pm\sqrt{(\Sigma-2)(\Sigma-4)}.}
$$

The roots are negative and real below $\Sigma=2$, coalesce at $-1$, and then form a complex-conjugate pair. For $2<\Sigma<4$ they trace the unit circle from $-1$ to $+1$; they cross the imaginary axis at $\lambda=\pm i$ when

$$
\boxed{\Sigma_c=3,}
$$

which is a [Hopf bifurcation](../../../../../hopf-bifurcation.md). Above $\Sigma=4$ they separate along the positive real axis.

Viscous drag and elastic spring forces alone have a symmetric positive mobility and a symmetric potential Hessian, so an overdamped gradient system has only real decay rates. The follower force is nonconservative: its linearized generalized-force matrix is nonsymmetric and cannot be derived from a potential. This broken variational structure permits complex eigenvalues and hence an oscillatory instability even though inertia is absent.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 355](../../paper-355-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
