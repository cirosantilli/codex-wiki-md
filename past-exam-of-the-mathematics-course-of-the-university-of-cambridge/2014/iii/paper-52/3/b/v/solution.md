<h1 id="3/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For the [scalar wave separation in Kerr spacetime](../../../../../../../scalar-wave-separation-in-kerr-spacetime.md), continue to use $A=r^2+a^2$ and $s=\sin\theta$. First verify the determinant in the hint. Direct multiplication of the covariant $t,\phi$ components gives

$$
\begin{aligned}
\Sigma^2(g_{tt}g_{\phi\phi}-g_{t\phi}^2)&=-s^2(\Delta-a^2s^2)(A^2-\Delta a^2s^2)-a^2s^4(A-\Delta)^2\\
&=-\Delta s^2(A-a^2s^2)^2=-\Delta s^2\Sigma^2.
\end{aligned}
$$

Hence the block determinant is $-\Delta\sin^2\theta$. Inverting this block gives

$$
g^{tt}=-\frac{A^2-\Delta a^2s^2}{\Sigma\Delta},\qquad g^{t\phi}=-\frac{a(A-\Delta)}{\Sigma\Delta},\qquad g^{\phi\phi}=\frac{\Delta-a^2s^2}{\Sigma\Delta s^2}.
$$

The other inverse components are $g^{rr}=\Delta/\Sigma$, $g^{\theta\theta}=1/\Sigma$, and $\sqrt{-g}=\Sigma s$. The [covariant wave operator](../../../../../../../covariant-wave-operator.md) on a scalar consequently has the divergence form

$$
\Box\Psi=\frac1{\Sigma s}\partial_\mu(\Sigma s\,g^{\mu\nu}\partial_\nu\Psi).
$$

Let $m_\phi$ denote the azimuthal mode number, to distinguish it from the axial vector $m$. Insert the mode $\Psi=e^{-i\omega t+i m_\phi\phi}R(r)\Theta(\theta)$ in the massless [Klein-Gordon equation](../../../../../../../klein-gordon-equation.md). Single-valuedness makes $m_\phi$ an integer. The $t,\phi$ derivatives give

$$
\Sigma\left(-\omega^2g^{tt}+2\omega m_\phi g^{t\phi}-m_\phi^2g^{\phi\phi}\right)=\frac{(A\omega-a m_\phi)^2}{\Delta}+2a\omega m_\phi-a^2\omega^2\sin^2\theta-\frac{m_\phi^2}{\sin^2\theta}.
$$

With $K(r)=A\omega-a m_\phi$, division by the mode factor gives, on patches where $R\Theta\ne0$,

$$
\frac{(\Delta R')'}R+\frac{K^2}\Delta+2a\omega m_\phi-a^2\omega^2+\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}+a^2\omega^2\cos^2\theta-\frac{m_\phi^2}{\sin^2\theta}=0.
$$

The radial and angular expressions must be opposite constants. Defining the [separation constant](../../../../../../../separation-constant.md) as $\Lambda$, we obtain the two [ordinary differential equations](../../../../../../../ordinary-differential-equation.md)

$$
\boxed{\frac1{\sin\theta}\frac d{d\theta}\left(\sin\theta\frac{d\Theta}{d\theta}\right)+\left(a^2\omega^2\cos^2\theta-\frac{m_\phi^2}{\sin^2\theta}+\Lambda\right)\Theta=0,}
$$



$$
\boxed{\frac d{dr}\left(\Delta\frac{dR}{dr}\right)+\left[\frac{((r^2+a^2)\omega-a m_\phi)^2}{\Delta}-a^2\omega^2+2a\omega m_\phi-\Lambda\right]R=0.}
$$

These equations also hold at zeros of a mode by continuity, without dividing there. Regular angular solutions are [scalar spheroidal harmonics](../../../../../../../scalar-spheroidal-harmonic.md), with discrete $\Lambda=\Lambda_{\ell m_\phi}(a\omega)$. For $a\omega=0$ the angular equation becomes the [associated Legendre function](../../../../../../../associated-legendre-function.md) equation, with $\Lambda=\ell(\ell+1)$ and $\ell\geq|m_\phi|$, providing a useful check of the signs and normalization. The radial function here is exactly $R$ in the chosen ansatz, without an additional factor of $1/r$.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 52](../../../../paper-52-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
