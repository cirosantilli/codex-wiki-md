<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Invariant distribution of an Itô diffusion](../../../../../../invariant-distribution-of-an-ito-diffusion.md), specialized to [Underdamped Langevin dynamics](../../../../../../underdamped-langevin-dynamics.md), has density

$$
\pi(x,p)=Z^{-1}\exp\left\{-U(x)-\frac{\lVert p\rVert^2}{2\eta}\right\}.
$$

Thus $X$ has density proportional to $e^{-U(x)}$, and conditionally and marginally $P\sim N(0,\eta I_d)$. The Hamiltonian transport between $x$ and $p$ preserves this density, while the [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md) in momentum has exactly that Gaussian invariant law.

The [Euler-Maruyama method](../../../../../../euler-maruyama-method.md) with step size $\delta$ and independent $\xi_k\sim N(0,I_d)$ is

$$
\begin{aligned}
P_{k+1}
&=P_k-\gamma\delta P_k-\eta\delta\nabla U(X_k)
+\sqrt{2\gamma\eta\delta}\,\xi_k,\\
X_{k+1}&=X_k+\delta P_k.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
