<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $C=N_0n$ be the cell number density. The steady [cell conservation equation](../../../../../../cell-conservation-in-a-swimming-suspension.md) with isotropic translational [diffusion](../../../../../../diffusion.md) is

$$
\nabla\cdot\left[n(\mathbf u+V_s\langle\mathbf p\rangle)-D\nabla n\right]=0.
$$

Using the [rapid-rotation mean gyrotactic orientation](../../../../../../rapid-rotation-mean-gyrotactic-orientation.md), put $a_s=2V_s/(3B\Omega)$, so the swimming drift is $-a_s\mathbf e_1$. In the transverse plane, $x_1=Rr\cos\theta'$ and $x_3=Rr\sin\theta'$. Thus $\mathbf u\cdot\nabla=\Omega\partial_{\theta'}$ and

$$
\partial_{x_1}=\frac1R\left(\cos\theta'\,\partial_r-\frac{\sin\theta'}r\partial_{\theta'}\right).
$$

Multiplying the conservation equation by $-R^2/D$ gives

$$
\boxed{n_{rr}+\frac1rn_r+\frac1{r^2}n_{\theta'\theta'}-\beta^2n_{\theta'}+\varepsilon\left(\cos\theta'\,n_r-\frac{\sin\theta'}r n_{\theta'}\right)=0,}
$$

with $\beta^2=\Omega R^2/D$ and $\varepsilon=a_sR/D=2V_sR/(3B\Omega D)$. The base fluid [velocity](../../../../../../velocity.md) is tangent to the wall. Zero normal cell flux there is $-a_sn\cos\theta'-Dn_r/R=0$, or

$$
\boxed{n_r+\varepsilon n\cos\theta'=0\quad(r=1).}
$$

Normalization requires the cross-sectional mean of $n$ to be one.

For $\varepsilon\ll1$, set $n=1+\varepsilon\operatorname{Re}[a(r)e^{i\theta'}]+O(\varepsilon^2)$. The drift term acting on the leading constant vanishes, and the first angular harmonic satisfies

$$
a''+\frac1ra'-\frac1{r^2}a-i\beta^2a=0,\qquad a'(1)=-1.
$$

Writing $q=e^{i\pi/4}\beta$ turns this into the [Modified Bessel differential equation](../../../../../../modified-bessel-differential-equation.md) of order one. Its regular solution is

$$
\boxed{a(r)=-\frac{I_1(qr)}{qI_1'(q)},}
$$

where $I_1$ is the [Modified Bessel function of the first kind](../../../../../../modified-bessel-function-of-the-first-kind.md). The singular second solution is excluded at the axis, and the displayed coefficient enforces the wall [boundary condition](../../../../../../boundary-condition.md). The angular harmonic has zero area average, so the normalization is satisfied at this order.

When $\beta\gg1$, the [gyrotactic concentration layer at a rotating-cylinder wall](../../../../../../gyrotactic-concentration-layer-at-a-rotating-cylinder-wall.md) has stretched coordinate $s=\beta(1-r)$. The leading radial equation is $a_{ss}-ia=0$. The solution decaying into the interior is proportional to $e^{-e^{i\pi/4}s}$; the wall condition fixes its coefficient to $-1/q$. Hence

$$
\boxed{n\simeq1-\frac\varepsilon\beta\operatorname{Re}\left[e^{i(\theta'-\pi/4)}\exp\{-e^{i\pi/4}\beta(1-r)\}\right].}
$$

This also follows from the large-argument [asymptotic expansion](../../../../../../asymptotic-expansion.md) of $I_1$, which gives $a\sim-r^{-1/2}e^{-q(1-r)}/q$ near the wall; $r^{-1/2}=1+O(\beta^{-1})$ within the layer. Its thickness is $R/\beta=\sqrt{D/\Omega}$. The quoted exponential is a wall-layer approximation, not an exact solution all the way to $r=0$; the [Modified Bessel function of the first kind](../../../../../../modified-bessel-function-of-the-first-kind.md) formula supplies the regular continuation through the axis.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
