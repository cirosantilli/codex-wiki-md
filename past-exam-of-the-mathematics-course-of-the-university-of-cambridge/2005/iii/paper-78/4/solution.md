<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [spin tensor](../../../../../spin-tensor.md) $W$ is skew, and $\dot Q Q^T=W$ means $\dot Q=WQ$ and $\dot Q^T=-Q^TW$. Differentiate all factors to obtain the [corotating-frame representation of a Jaumann derivative](../../../../../corotating-frame-representation-of-a-jaumann-derivative.md):

$$
\begin{aligned}
\frac d{dt}(Q^TTQ)
&=-Q^TWTQ+Q^T\dot TQ+Q^TTWQ\\
&=Q^T(\dot T-WT+TW)Q.
\end{aligned}
$$

Thus the [Jaumann derivative](../../../../../jaumann-derivative.md) is the ordinary derivative of the [tensor](../../../../../tensor.md) components in this rotating frame.

Put $S=\sigma^d$, $\Delta\mu=\mu_1-\mu_0$, $A=S-2\mu_0D$ and $\widetilde A=Q^TAQ$, $\widetilde D=Q^TDQ$. The [corotational Jeffreys fluid](../../../../../corotational-jeffreys-fluid.md) equation reduces to

$$
\dot{\widetilde A}+\frac1\tau\widetilde A
=\frac{2\Delta\mu}{\tau}\widetilde D.
$$

For $\tau>0$, an [integrating factor](../../../../../integrating-factor.md) gives the complete finite-initial-time solution

$$
\widetilde A(t)=e^{-(t-t_0)/\tau}\widetilde A(t_0)
+\frac{2\Delta\mu}{\tau}\int_{t_0}^t
 e^{-(t-s)/\tau}\widetilde D(s)\,ds.
$$

The infinite-past constitutive history selects $\lim_{t_0\to-\infty}e^{t_0/\tau}\widetilde A(t_0)=0$, as holds for bounded past [stress](../../../../../stress.md) histories, and assumes convergence of the integral. Taking that limit and rotating back proves

$$
\boxed{S(t)=2\mu_0D(t)+\frac{2\Delta\mu}{\tau}
\int_{-\infty}^t e^{-(t-s)/\tau}
Q(t)Q^T(s)D(s)Q(s)Q^T(t)\,ds.}
$$

A general initial [stress](../../../../../stress.md) would retain the displayed homogeneous term. [Incompressibility](../../../../../incompressible-flow.md) means $\operatorname{tr}D=0$; the [pressure](../../../../../pressure.md) reaction is added as $\sigma=S-pI$ and does not affect this [deviatoric stress](../../../../../deviatoric-stress.md) equation.

For [simple shear deformation](../../../../../simple-shear.md), direct multiplication gives the [velocity gradient](../../../../../velocity-gradient.md) and its symmetric and skew parts:

$$
L=\dot FF^{-1}=\begin{pmatrix}0&\dot\gamma\\0&0\end{pmatrix},\qquad
D=\frac{\dot\gamma}{2}\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
W=\frac{\dot\gamma}{2}\begin{pmatrix}0&1\\-1&0\end{pmatrix}.
$$

Use the signed counterclockwise angle $\theta$ with

$$
Q(t)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix},
\qquad \dot\theta=-\dot\gamma/2.
$$

Thus the material frame rotates clockwise for positive shear rate. This angle convention is necessary for the signs of the sine terms. Set $\delta=\theta(t)-\theta(s)$. With $H=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and $R_\delta=Q(t)Q^T(s)$, multiplication yields

$$
R_\delta H R_\delta^T
=\begin{pmatrix}-\sin2\delta&\cos2\delta\\
\cos2\delta&\sin2\delta\end{pmatrix}.
$$

Substitution in the history formula proves

$$
\boxed{S(t)=\mu_0\dot\gamma(t)H+
\frac{\Delta\mu}{\tau}\int_{-\infty}^t
 e^{-(t-s)/\tau}\dot\gamma(s)
\begin{pmatrix}-\sin2\delta&\cos2\delta\\
\cos2\delta&\sin2\delta\end{pmatrix}ds.}
$$

The suppressed third row and column are zero for the selected infinite-past history.

For constant shear rate $g=\dot\gamma$, $2\delta=-g(t-s)$. Put $u=t-s\geq0$. The real and imaginary parts of the elementary exponential integral give

$$
\int_0^\infty e^{-u/\tau}\cos(gu)\,du
=\frac\tau{1+g^2\tau^2},\qquad
\int_0^\infty e^{-u/\tau}\sin(gu)\,du
=\frac{g\tau^2}{1+g^2\tau^2}.
$$

The constant-rate [deviatoric stress](../../../../../deviatoric-stress.md) therefore has components

$$
\boxed{S_{12}=\frac{\mu_1+\mu_0g^2\tau^2}{1+g^2\tau^2}\,g,\qquad
S_{11}=\frac{(\mu_1-\mu_0)g^2\tau}{1+g^2\tau^2},\qquad
S_{22}=-S_{11}.}
$$

The [normal-stress difference](../../../../../normal-stress-difference.md) is $2(\mu_1-\mu_0)g^2\tau/(1+g^2\tau^2)$. As checks, the small-rate shear viscosity is $\mu_1$, and $\mu_1=\mu_0$ removes all memory and normal [stresses](../../../../../stress.md), leaving the Newtonian relation $S=2\mu_0D$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
