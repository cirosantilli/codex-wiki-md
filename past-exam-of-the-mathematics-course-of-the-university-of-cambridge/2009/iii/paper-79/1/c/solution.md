<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The rigid bottom reflects the lower-layer wave. Its repeated returns to the interface create an [internal-wave cavity response](../../../../../../internal-wave-cavity-response.md) containing both upward and downward components in $-H<z<0$, while the upper layer contains the imposed incident wave and one net reflected wave.

Let the lower downward and upward particle-displacement coefficients be $D$ and $U$, multiplying $e^{im_2z}$ and $e^{-im_2z}$ respectively. Their vertical displacement has opposite polarization signs:

$$
\xi_z(z)=\cos\theta_2[-De^{im_2z}+Ue^{-im_2z}].
$$

Zero normal velocity at $z=-H$ gives $U=Dq$, where $q=e^{-2im_2H}$. Interface continuity consequently becomes

$$
\sin\theta_1(\eta_i+\eta_r)=\sin\theta_2D(1+q),\qquad
\cos\theta_1(\eta_i-\eta_r)=\cos\theta_2D(1-q).
$$

For the specified angles, $\sin\theta_2/\sin\theta_1=1/\sqrt3$ and $\cos\theta_2/\cos\theta_1=\sqrt3$. Thus

$$
\frac D{\eta_i}=\frac{\sqrt3}{2-e^{-2im_2H}},\qquad
\frac{\eta_r}{\eta_i}=\frac{-1+2e^{-2im_2H}}{2-e^{-2im_2H}}.
$$

The dependence on bottom depth is therefore

$$
\boxed{|D|=|U|=\frac{\sqrt3|\eta_i|}{\sqrt{1+8\sin^2(m_2H)}}.}
$$

In particular,

$$
\boxed{|D|_{\max}=\sqrt3|\eta_i|\quad\text{when }m_2H=n\pi.}
$$

Here $k=\pi/\lambda_i$ and $m_2=k/\sqrt3$, so the positive depths giving this maximum are

$$
\boxed{H=n\sqrt3\lambda_i,\qquad n=1,2,\ldots.}
$$

The lower vertical-displacement standing-wave envelope is $2\cos\theta_2|D|\,|\sin[m_2(z+H)]|$, while its horizontal-displacement envelope has the complementary cosine form. These distinguish the total standing disturbance from the amplitude of either traveling component. The traveling amplitude has minimum $|\eta_i|/\sqrt3$ at $m_2H=(n+1/2)\pi$.

Since $|q|=1$, $|-1+2q|=|2-q|$. Hence **the net upward-propagating wave in the upper layer has amplitude magnitude $|\eta_i|$ for every $H$**, with the phase given above. At an enhancement maximum, $q=1$ and $\eta_r=\eta_i$. No energy escapes through the bottom, so complete eventual reflection is consistent with energy conservation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
