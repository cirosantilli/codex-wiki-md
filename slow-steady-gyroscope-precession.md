# Slow steady gyroscope precession

↑ **Parent:** [Gyroscope](gyroscope.md)

Model the assembly as a [heavy symmetric top](heavy-symmetric-top.md) with a fixed frictionless support, a uniform [gravitational field](gravitational-field.md), and [centre of mass](center-of-mass.md) on its symmetry axis. Assume constant spin, negligible [damping](damping.md), and initial conditions prepared for [uniform precession of a heavy symmetric top](uniform-precession-of-a-heavy-symmetric-top.md). Large spin means the transverse [angular momentum](angular-momentum.md) from [precession](precession.md) is small: $I_1|\Omega|\sin\theta\ll|I_3\omega_3|$. Also require $|\Omega|\ll|\omega_3|$. A large spin rate alone does not select steady motion after an arbitrary release.

For an original illustrative calculation, stipulate

$$
M=2.0\,\mathrm{kg},\quad d=0.15\,\mathrm m,\quad g=9.81\,\mathrm{m/s^2},\quad
I_3=0.080\,\mathrm{kg\,m^2},\quad I_1=I_2=0.090\,\mathrm{kg\,m^2},\quad
\omega_3=100\,\mathrm{rad/s},\quad\theta=60^\circ.
$$

The transverse [principal moments of inertia](principal-moment-of-inertia.md) $I_1,I_2$ are about the pivot, including the [parallel axis theorem](parallel-axis-theorem.md) contribution. These inputs give

$$
L_s=8.0\,\mathrm{kg\,m^2/s},\quad K=Mgd=2.943\,\mathrm{N\,m},\quad
|\boldsymbol\tau_O|=K\sin60^\circ=2.5487\,\mathrm{N\,m},
$$



$$
\Omega_0=K/L_s=0.367875\,\mathrm{rad/s},\qquad T_0=2\pi/\Omega_0\simeq17.080\,\mathrm s.
$$

The ratio $\Omega_0/\omega_3=0.00368$ is small; the more direct [angular momentum](angular-momentum.md) ratio $I_1\Omega_0\sin60^\circ/L_s=0.00358$ is small too. These are model calculations, not experimental results.

Check the approximation against the existing exact [uniform precession of a heavy symmetric top](uniform-precession-of-a-heavy-symmetric-top.md) condition. Its total [angular momentum](angular-momentum.md) is

$$
\mathbf L_O=I_1\Omega(\widehat{\mathbf z}-\cos\theta\widehat{\mathbf e})+L_s\widehat{\mathbf e}.
$$

At constant $\theta,\Omega,L_s$, differentiating this expression and equating it to the gravitational [torque](torque.md) gives

$$
I_1\cos\theta\,\Omega^2-L_s\Omega+K=0.
$$

For $L_s>0$ the slow solution can be evaluated without subtracting two nearly equal numbers:

$$
\Omega_{\mathrm{slow}}=\frac{2K}{L_s+\sqrt{L_s^2-4I_1K\cos\theta}}
\simeq0.368639\,\mathrm{rad/s}.
$$

It exceeds $\Omega_0$ by about $0.208\%$. The other solution is about $177.409\,\mathrm{rad/s}$ and violates the assumed slow [precession](precession.md); the quadratic's two roots must not be conflated. Its [discriminant](discriminant.md) must be nonnegative for these steady solutions to exist.

<a id="image-synthetic-steady-precession-calculations-larger-spin-slows-the-drift-and-larger-transverse-torque-speeds-it-up"></a>
![](gyroscope-precession-spin-torque-sweep.png)

**[Figure 22](#image-synthetic-steady-precession-calculations-larger-spin-slows-the-drift-and-larger-transverse-torque-speeds-it-up). Synthetic steady-precession calculations: larger spin slows the drift and larger transverse torque speeds it up**.

The original curves hold $I_1,I_3,\theta$ fixed and vary spin and the imposed [torque](torque.md) coefficient $K$ in $\boldsymbol\tau_O=K\widehat{\mathbf z}\times\widehat{\mathbf e}$. For gravity alone, $K=Mgd$; the other curves are hypothetical changes in the transverse [torque](torque.md), not observations of this wheel. Solid curves use the slow quadratic root; dashed curves use $K/(I_3\omega_3)$. The second panel displays their relative difference. Increasing spin improves this approximation for the parameters shown. It does not remove [nutation](nutation.md) caused by inappropriate initial conditions.

## ↑ Ancestors (7)

1. [Gyroscope](gyroscope.md)
2. [Angular momentum](angular-momentum.md)
3. [Momentum](momentum.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gyroscope](gyroscope.md)
