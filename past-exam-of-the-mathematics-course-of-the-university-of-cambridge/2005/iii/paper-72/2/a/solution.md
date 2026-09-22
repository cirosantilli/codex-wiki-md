<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $V=|\mathbf V|$ to be the test body's instantaneous [speed](../../../../../../speed.md) relative to the nonstreaming background, rather than an ensemble [root mean square](../../../../../../root-mean-square.md) [speed](../../../../../../speed.md). Use a local isotropic [galactic distribution function](../../../../../../galactic-distribution-function.md) $f(v)$ normalized as a number distribution, and assume independent encounters and a large, approximately constant [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md).

For a background particle with relative incoming [velocity](../../../../../../velocity.md) $\mathbf w=\mathbf V-\mathbf v$, a [gravitational scattering angle](../../../../../../gravitational-scattering-angle.md) $\chi$ obeys

$$
\tan(\chi/2)=\frac{G(M+m)}{bw^2}=\frac{b_{90}}b.
$$

In the [centre-of-momentum frame](../../../../../../center-of-momentum-frame.md), the test body's share of the relative [velocity](../../../../../../velocity.md) is $m/(M+m)$. The azimuthal average cancels transverse changes, leaving a change parallel to the incoming relative [velocity](../../../../../../velocity.md),

$$
\Delta\mathbf V_\parallel=-\frac{m}{M+m}(1-\cos\chi)\mathbf w=-\frac{2m}{M+m}\frac{\mathbf w}{1+b^2/b_{90}^2}.
$$

The number of encounters per unit time in $d^3v$ and impact interval $db$ is $f(v)d^3v\,w\,2\pi b\,db$. Integrating the longitudinal change from $b=0$ to $b_m$ gives

$$
\dot{\mathbf V}=-2\pi G^2m(M+m)\int f(v)\frac{\mathbf w}{w^3}\log\!\left(1+\frac{b_m^2w^4}{G^2(M+m)^2}\right)d^3v.
$$

At leading logarithmic order replace the logarithm by $2\ln\Lambda$, evaluated at a representative [speed](../../../../../../speed.md). For isotropic $f$, the [velocity-shell identity for dynamical friction](../../../../../../velocity-shell-identity-for-dynamical-friction.md) is

$$
\int f(v)\frac{\mathbf V-\mathbf v}{|\mathbf V-\mathbf v|^3}\,d^3v=\frac{4\pi\mathbf V}{V^3}\int_0^Vf(v)v^2\,dv.
$$

One proof takes the divergence with respect to $\mathbf V$: the inverse-square [vector field](../../../../../../vector-field.md) has divergence $4\pi\delta^{(3)}(\mathbf V-\mathbf v)$, whose velocity integral is $4\pi f(V)$, and [rotational symmetry](../../../../../../rotational-symmetry.md) plus the [divergence theorem](../../../../../../divergence-theorem.md) determines the radial field. Exterior [velocity](../../../../../../velocity.md) shells give zero field. Consequently the systematic [Chandrasekhar dynamical friction](../../../../../../chandrasekhar-dynamical-friction.md) is antiparallel to motion, with

$$
\dot V=-\frac{16\pi^2G^2m(M+m)\ln\Lambda}{V^2}\int_0^Vf(v)v^2\,dv.
$$

In the massive-test-body approximation $M\gg m$, this becomes

$$
\boxed{\dot V=-\frac{16\pi^2G^2mM\ln\Lambda}{V^2}\int_0^Vf(v)v^2\,dv,\qquad \Lambda=\frac{b_mV^2}{GM}.}
$$

The [finite-test-mass dynamical friction coefficient](../../../../../../finite-test-mass-dynamical-friction-coefficient.md) shows the needed qualification: $M>m$ alone does not make $M+m=M$. The quoted expression also neglects diffusion and the [velocity](../../../../../../velocity.md) dependence of the logarithmic cutoff. For the [lowered Maxwellian velocity distribution](../../../../../../lowered-maxwellian-velocity-distribution.md), set $f=0$ for $v>v_e$; continuing the printed subtraction beyond escape would give a negative distribution. If $V>v_e$, the integral stops at $v_e$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
