<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Normalizing the true density gives

$$
f(x)=\frac{\sqrt\beta}{\sqrt\pi}x^{-1/2}e^{-\beta x}\qquad(x>0),
$$

a [gamma distribution](../../../../../../gamma-distribution.md) of shape $1/2$ and rate $\beta$. Its mean is $1/(2\beta)=\mu$, and the [Gamma integral](../../../../../../gamma-integral.md) gives

$$
M_X(r)=\left(1-\frac r\beta\right)^{-1/2}\qquad(0\leq r<\beta).
$$

Put $x=R/\beta$. Since $\mu\beta=1/2$, the positive [adjustment coefficient](../../../../../../adjustment-coefficient.md) satisfies

$$
(1-x)^{-1/2}=1+\frac{1+\rho}{2}x,\qquad0<x<1.
$$

Both sides are positive in this domain. Squaring, multiplying by $1-x$, and dividing out the zero root $x=0$ yields

$$
(1+\rho)^2x^2-(1+\rho)(\rho-3)x-4\rho=0.
$$

The discriminant is $(1+\rho)^2[(\rho-3)^2+16\rho]=(1+\rho)^2(\rho+9)(\rho+1)$. The negative constant term makes one root positive and the other negative. The polynomial is negative at zero and has value four at one, so the positive root lies in $(0,1)$ and is not an extraneous solution introduced by squaring. Therefore the [adjustment coefficient for shape-one-half gamma claims](../../../../../../adjustment-coefficient-for-shape-one-half-gamma-claims.md) is

$$
\boxed{R=\beta\frac{\rho-3+\sqrt{(\rho+9)(\rho+1)}}{2(1+\rho)}.}
$$

To compare it with the exponential calculation, write $R_I=2\beta\rho/(1+\rho)$. Their difference is

$$
R_I-R=\frac\beta{2(1+\rho)}\left[3(1+\rho)-\sqrt{(\rho+9)(\rho+1)}\right]>0,
$$

since $9(1+\rho)^2-(\rho+9)(\rho+1)=8\rho(1+\rho)>0$. Thus the two proposed [Lundberg inequality](../../../../../../lundberg-inequality.md) bounds are ordered as

$$
\boxed{0<R<R_I,\qquad e^{-R_Iu}<e^{-Ru}\quad(u>0).}
$$

Only $\psi_{\rm true}(u)\leq e^{-Ru}$ is justified for the true claim law. The exponential calculation gives $\psi_{\rm exponential}(u)\leq e^{-R_Iu}$ for a different model, not a valid guaranteed bound on the true ruin probability.

This [exponential misspecification of shape-one-half gamma claims](../../../../../../exponential-misspecification-of-shape-one-half-gamma-claims.md) is optimistic: the true [variance](../../../../../../variance-split.md) is $1/(2\beta^2)=2\mu^2$, whereas the assumed exponential [variance](../../../../../../variance-split.md) is $\mu^2$. Its tail also decays at rate $\beta$, more slowly than the assumed rate $1/\mu=2\beta$. Equivalently, for $0<r<\beta$, the true transform $(1-2\mu r)^{-1/2}$ is larger than $(1-\mu r)^{-1}$, since $(1-\mu r)^2>1-2\mu r$. This stronger transform growth makes the true adjustment root smaller. Comparing upper bounds alone does not by itself prove an ordering of the two actual ruin probabilities. At $u=0$ both displayed bounds equal one.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
