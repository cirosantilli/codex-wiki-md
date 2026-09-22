<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Differentiate the pulled-back [Kirchhoff stress tensor](../../../../../kirchhoff-stress-tensor.md) $T=F^T\tau F$, using the [velocity gradient](../../../../../velocity-gradient.md) convention $L=\dot FF^{-1}$:

$$
\dot T=\dot F^T\tau F+F^T\dot\tau F+F^T\tau\dot F=F^T(\dot\tau+L^T\tau+\tau L)F.
$$

Thus the [lower-convected stress pull-back](../../../../../lower-convected-stress-pull-back.md) gives

$$
\boxed{\mathcal D_l\tau=\dot\tau+L^T\tau+\tau L=F^{-T}\dot TF^{-1}}.
$$

For an explicit [objective time derivative](../../../../../objective-time-derivative.md) check, superpose $x^*=Q(t)x+c(t)$, with $Q^TQ=I$ and $\Omega=\dot QQ^T$ skew. Then $\tau^*=Q\tau Q^T$ and $L^*=QLQ^T+\Omega$, whereas

$$
\dot\tau^*=Q\dot\tau Q^T+\Omega\tau^*-\tau^*\Omega.
$$

The additional terms in $(L^*)^T\tau^*+\tau^*L^*$ are $-\Omega\tau^*+\tau^*\Omega$. They cancel the extra material-derivative terms, proving $\boxed{\mathcal D_l\tau^*=Q(\mathcal D_l\tau)Q^T}$. The translation has no effect on a stress or velocity gradient.

For the incompressible [Oldroyd-A model](../../../../../oldroyd-a-model.md), avoid using the same symbol for a stress tensor and its relaxation time by referring to $\tau>0$ below only as the scalar relaxation time. Define $S=\sigma^d-2\mu_rD$. The constitutive equation becomes

$$
\mathcal D_lS+S/\tau=2(\mu-\mu_r)D/\tau.
$$

By the pull-back identity, $A=F^TSF$ satisfies

$$
\dot A+A/\tau=2(\mu-\mu_r)F^TDF/\tau.
$$

An [integrating factor](../../../../../integrating-factor.md) gives

$$
A(t)=e^{-(t-t_0)/\tau}A(t_0)+\frac{2(\mu-\mu_r)}\tau\int_{t_0}^t e^{-(t-s)/\tau}F(s)^TD(s)F(s)\,ds.
$$

Push forward by $F(t)^{-T}$ and $F(t)^{-1}$. For a convergent, fading remote-past history with the transported homogeneous term tending to zero as $t_0\to-\infty$, this proves the [fading-memory representation of the Oldroyd-A model](../../../../../fading-memory-representation-of-the-oldroyd-a-model.md):

$$
\boxed{\sigma^d(t)=2\mu_rD(t)+\frac{2(\mu-\mu_r)}\tau\int_{-\infty}^t e^{-(t-s)/\tau}F(t)^{-T}F(s)^TD(s)F(s)F(t)^{-1}\,ds}.
$$

For arbitrary finite-time initial data retain $e^{-(t-t_0)/\tau}F(t)^{-T}A(t_0)F(t)^{-1}$. Thus the printed integral-only expression incorporates an initial-memory condition; it is not an unconditional replacement for all initial-value solutions.

For time-dependent [simple shear](../../../../../simple-shear.md),

$$
L=\begin{pmatrix}0&\dot\gamma(t)\\0&0\end{pmatrix},\qquad D(t)=\frac{\dot\gamma(t)}2\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Put $\Delta\gamma=\gamma(s)-\gamma(t)$. The relative deformation is $F(s)F(t)^{-1}=\begin{pmatrix}1&\Delta\gamma\\0&1\end{pmatrix}$, so the entire transported integrand simplifies to

$$
F(t)^{-T}F(s)^TD(s)F(s)F(t)^{-1}=\frac{\dot\gamma(s)}2\begin{pmatrix}0&1\\1&2\Delta\gamma\end{pmatrix}.
$$

Consequently the explicit nonpressure stresses are

$$
\boxed{\begin{aligned}
\sigma_{11}^d(t)&=0,\\
\sigma_{12}^d(t)&=\mu_r\dot\gamma(t)+\frac{\mu-\mu_r}{\tau}\int_{-\infty}^t e^{-(t-s)/\tau}\dot\gamma(s)\,ds,\\
\sigma_{22}^d(t)&=\frac{2(\mu-\mu_r)}\tau\int_{-\infty}^t e^{-(t-s)/\tau}\dot\gamma(s)[\gamma(s)-\gamma(t)]\,ds.
\end{aligned}}
$$

Symmetry gives $\sigma_{21}^d=\sigma_{12}^d$, and the unshown third-direction nonpressure components vanish. The superscript $d$ here labels the paper's nonpressure constitutive stress; it need not have zero trace. Subtracting $pI$ supplies the total [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md).

For constant shear rate $s_0$, use $\gamma(s)-\gamma(t)=-s_0(t-s)$ and the integrals $\int_0^\infty e^{-a/\tau}da=\tau$ and $\int_0^\infty ae^{-a/\tau}da=\tau^2$. This gives the [steady simple shear of an Oldroyd-A fluid](../../../../../steady-simple-shear-of-an-oldroyd-a-fluid.md) result

$$
\sigma_{12}^d=\mu s_0,\qquad \sigma_{22}^d=-2(\mu-\mu_r)\tau s_0^2,\qquad \sigma_{11}^d=0,
$$

and therefore

$$
\boxed{\sigma_{11}-\sigma_{22}=2(\mu-\mu_r)\tau s_0^2}.
$$

The incompressibility pressure cancels from this [normal-stress difference](../../../../../normal-stress-difference.md). With the usual $\mu\geq\mu_r\geq0$, it is nonnegative, while the second normal-stress difference equals its negative.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
