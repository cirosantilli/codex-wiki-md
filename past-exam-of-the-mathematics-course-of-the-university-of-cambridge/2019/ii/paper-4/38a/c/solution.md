<h1 id="38a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The obstacle and wave pattern are stationary, so $\omega=\Omega=0$. With

$$
(k_1,k_2)=\kappa(\cos\phi,\sin\phi),
\qquad \kappa>0,
$$

the dispersion relation becomes

$$
0=\alpha\kappa^{1/2}-V\kappa\cos\phi.
$$

Hence $\cos\phi>0$, so $-\pi/2<\phi<\pi/2$, and

$$
\boxed{\kappa=\frac{\alpha^2}{V^2\cos^2\phi}.}
$$

Differentiating the dispersion relation with respect to the wavevector gives

$$
\begin{aligned}
\mathbf c_g
=\nabla_{\mathbf k}\Omega
&=\frac{\alpha}{2\sqrt\kappa}
(\cos\phi,\sin\phi)-(V,0)\\
&=\frac V2\left(\cos^2\phi-2,\,
\sin\phi\cos\phi\right),
\end{aligned}
$$

where the zero-frequency relation  
$\alpha/\sqrt\kappa=V\cos\phi$ was used. Its first component is always negative, so the ray angle $\psi$ lies in

$$
\frac\pi2<\psi<\frac{3\pi}{2}.
$$

Moreover,

$$
\boxed{
\tan\psi
=\frac{\sin\phi\cos\phi}{\cos^2\phi-2}
=-\frac{\tan\phi}{1+2\tan^2\phi}.}
$$

Put $q=|\tan\phi|$. The magnitude of the slope relative to the negative $x_1$-axis is

$$
F(q)=\frac{q}{1+2q^2}.
$$

Its [derivative](../../../../../../derivative.md) is

$$
F'(q)=\frac{1-2q^2}{(1+2q^2)^2},
$$

so its [global maximum](../../../../../../global-maximum.md) occurs at $q=1/\sqrt2$ and equals

$$
F_{\max}=\frac1{2\sqrt2}=2^{-3/2}.
$$

Therefore all group-velocity rays lie in the [stationary square-root-dispersion wake](../../../../../../stationary-square-root-dispersion-wake.md)

$$
\boxed{
|\psi-\pi|\leq\tan^{-1}(2^{-3/2}),}
$$

a wedge of semi-angle $\tan^{-1}(2^{-3/2})$ extending in the negative $x_1$-direction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [38A](../../38a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
