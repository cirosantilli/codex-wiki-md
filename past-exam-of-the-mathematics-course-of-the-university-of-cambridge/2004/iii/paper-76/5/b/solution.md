<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume again positive [diffusion](../../../../../../diffusion.md) $\gamma>0$. Remove the drift with $A(x,t)=e^{Ux/(2\gamma)-i\omega t}f(x)$. Differentiating explicitly cancels the first [derivative](../../../../../../derivative.md) and gives

$$
\gamma f''+\left[\mu_0-\frac{U^2}{4\gamma}-\epsilon\lambda x+i\omega\right]f=0.
$$

Balance the second [derivative](../../../../../../derivative.md) with the linear confinement by taking $x=O(\epsilon^{-1/3})$, so the requested exponent is **$\sigma=1/3$**. More precisely, put

$$
\xi=\left(\frac{\epsilon\lambda}{\gamma}\right)^{1/3}x,\qquad
\Lambda=(\epsilon^2\gamma\lambda^2)^{1/3},\qquad
c=\frac{\mu_0-U^2/(4\gamma)+i\omega}{\Lambda}.
$$

The [eigenvalue problem](../../../../../../eigenvalue-problem.md) reduces to $f_{\xi\xi}=(\xi-c)f$. Its two solutions are [Airy functions](../../../../../../airy-function.md). The growing $\operatorname{Bi}(\xi-c)$ is excluded by the condition at infinity: its growth proportional to $e^{2\xi^{3/2}/3}$ dominates any linear-in-$x$ drift factor. The decaying $\operatorname{Ai}(\xi-c)$ remains admissible even after multiplication by $e^{Ux/(2\gamma)}$. The wall imposes $\operatorname{Ai}(-c)=0$, so $-c=z_n$, giving the [Airy global modes of a linearly confined Ginzburg-Landau equation](../../../../../../airy-global-modes-of-a-linearly-confined-ginzburg-landau-equation.md):

$$
\boxed{\omega_n=i\left[\mu_0-\frac{U^2}{4\gamma}+\Lambda z_n\right]},\qquad
A_n(x,t)=C_n e^{Ux/(2\gamma)-i\omega_nt}\operatorname{Ai}(\xi+z_n).
$$

The least negative zero, $z_1\simeq-2.338107$, gives the largest temporal [growth rate](../../../../../../growth-rate.md). Hence

$$
\boxed{\text{global instability: }\mu_0>\frac{U^2}{4\gamma}+|z_1|(\epsilon^2\gamma\lambda^2)^{1/3}}.
$$

At equality the leading global [eigenmode](../../../../../../normal-mode.md) is neutral, and below it all these [eigenmodes](../../../../../../normal-mode.md) decay. In contrast, freezing the coefficients locally gives [absolute hydrodynamic instability](../../../../../../absolute-hydrodynamic-instability.md) wherever $\mu_0-\epsilon\lambda x>U^2/(4\gamma)$. Such a pocket exists iff $\mu_0>U^2/(4\gamma)$ and extends to $x_a=[\mu_0-U^2/(4\gamma)]/(\epsilon\lambda)$. Thus global instability implies a locally absolutely unstable pocket, while the converse fails: a pocket shorter than $|z_1|(\gamma/(\epsilon\lambda))^{1/3}$ does not overcome the wall and confinement losses. The additional threshold is order $\epsilon^{2/3}$, precisely the loss produced by the [Airy function](../../../../../../airy-function.md) spatial scale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
