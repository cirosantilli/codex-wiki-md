<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The axisymmetric magnetic mode spans a one-dimensional real representation of axial rotations, so its signed amplitude is a real variable $B$. An equatorial dipole has two real horizontal components. Rotation through an angle $\vartheta$ rotates that pair; encoding the components by one [complex amplitude](../../../../../complex-amplitude.md) gives $A\mapsto e^{i\vartheta}A$, and rotation through $\pi$ gives $A\mapsto-A$. The velocity mode has the same rotational representation, so write it as $V\mapsto e^{i\vartheta}V$. Magnetic reversal acts as

$$
(B,A,V)\longmapsto(-B,-A,V).
$$

Thus the two relevant symmetries are axial rotation and magnetic reversal. Reflection symmetry has not been assumed, so complex coupling coefficients are permitted.

The equations for $B,A$ must be linear in the magnetic variables at fixed velocity. Combining this with rotational [equivariance](../../../../../equivariant-map.md), their general local form is

$$
\begin{aligned}
\dot B&=Bf(|V|^2)+A^*Vg(|V|^2)+AV^*g(|V|^2)^*,\\
\dot A&=Ah(|V|^2)+BVj(|V|^2)+A^*V^2\ell(|V|^2),
\end{aligned}
$$

where $f$ is real valued and $g,h,j,\ell$ are complex valued. These functions can be understood through their local Taylor expansions; the symmetry argument does not require a convergent infinite series. Reality of $\dot B$ explains its conjugate pairing.

For the velocity equation, a [monomial](../../../../../monomial.md) $B^pA^q(A^*)^rV^s(V^*)^t$ must have the same rotational weight as $V$ and be even under magnetic reversal. Its selection rules are

$$
q-r+s-t=1,\qquad p+q+r\text{ is even}.
$$

A formal sum of all such [monomials](../../../../../monomial.md) with complex coefficients is the most general local velocity evolution. At degree one there is $V$; at degree two there is $AB$; at degree three there are $V|V|^2,V|A|^2,V^*A^2,VB^2$. Expanding the magnetic equations similarly gives the [equivariant three-mode dynamo normal form](../../../../../equivariant-three-mode-dynamo-normal-form.md)

$$
\boxed{\begin{aligned}
\dot B&=\mu_1B+c_1A^*V+c_1^*AV^*-e|V|^2B,\\
\dot A&=(\mu_2+i\omega_2)A+c_2VB-d_2|V|^2A-d_3V^2A^*,\\
\dot V&=(\mu_3+i\omega_3)V+c_3AB-d_4V|V|^2-d_5V|A|^2-d_6V^*A^2-d_7VB^2.
\end{aligned}}
$$

The $\mu_i,\omega_i,e$ are real, and the remaining coefficients are complex. The minus signs on cubic coefficients are a convention, not an assumption about their signs. Terms such as $B^3$ and $A|A|^2$ are forbidden in the magnetic equations by magnetic linearity, even though symmetry alone would allow some of them.

For the [normalization of nonzero dynamo coupling coefficients](../../../../../normalization-of-nonzero-dynamo-coupling-coefficients.md), assume $c_1c_3\ne0$. Make the variable changes

$$
B=\widetilde B,\quad A=q e^{i\chi_A}\widetilde A,\quad V=v e^{i\chi_V}\widetilde V,
\qquad q=\frac1{\sqrt{|c_1c_3|}},\quad v=\sqrt{\frac{|c_3|}{|c_1|}},\quad\chi_V-\chi_A=-\arg c_1.
$$

The transformed coefficients are $\widetilde c_1=qv e^{i(\chi_V-\chi_A)}c_1=1$ and $\widetilde c_3=(q/v)e^{i(\chi_A-\chi_V)}c_3$, of modulus one. Thus

$$
\boxed{c_1=1,\qquad c_3=e^{i\beta},\qquad\beta=\arg(c_1^{\rm original}c_3^{\rm original}).}
$$

The remaining phase is genuine; the two complex coefficients cannot both generally be made positive real. A zero coupling cannot be normalized to one, so the printed normalization presupposes this generic nonzero-coupling case.

Now impose the specified simplification, in the normalized variables, and write $A=r e^{i\theta}$, $V=s e^{i\phi}$ with $r,s>0$ and signed real $B$. Put $\psi=\phi-\theta$. Separating real and imaginary parts gives

$$
\begin{aligned}
\dot B&=(\mu_1-es^2)B+2rs\cos\psi,\\
\dot r&=\mu_2r+c_2sB\cos\psi,\\
\dot s&=(\mu_3-d_4s^2)s+rB\cos(\beta-\psi),\\
\dot\theta&=\omega_2+\frac{c_2sB}{r}\sin\psi,\\
\dot\phi&=\omega_3+\frac{rB}{s}\sin(\beta-\psi),\\
\dot\psi&=\omega_3-\omega_2+\frac{rB}{s}\sin(\beta-\psi)-\frac{c_2sB}{r}\sin\psi.
\end{aligned}
$$

Constant moduli require the first three right sides to vanish. Since $rs\ne0$, the first equation also fixes $\cos\psi$, so a continuously evolving phase difference must be constant. Hence the last right side must vanish as well. Both phases then advance at one common frequency, giving a [relative equilibrium](../../../../../relative-equilibrium.md). These four algebraic conditions and the displayed common-frequency equations govern all the requested nonzero constant-modulus solutions, without needing to solve them.

The pure-velocity branch is

$$
B=A=0,\qquad V=s_0e^{i(\omega_3t+\phi_0)},\qquad s_0^2=\frac{\mu_3}{d_4}>0.
$$

This presumes $d_4\ne0$; the usual saturated branch has $\mu_3,d_4>0$. Near it, set $A=e^{i(\omega_3t+\phi_0)}(u+iv)$, $B=b$, and define $\Delta=\omega_2-\omega_3$ and $\kappa=\mu_1-es_0^2$. Magnetic feedback in the velocity equation is quadratic, so the first magnetic [linearization](../../../../../linearization.md) is

$$
\frac{d}{dt}\begin{pmatrix}b\\u\\v\end{pmatrix}
=\begin{pmatrix}\kappa&2s_0&0\\c_2s_0&\mu_2&-\Delta\\0&\Delta&\mu_2\end{pmatrix}
\begin{pmatrix}b\\u\\v\end{pmatrix}.
$$

A branch of the stated relative equilibria has a zero growth rate in this rotating frame. Its determinant therefore gives the [magnetic onset on a rotating velocity branch](../../../../../magnetic-onset-on-a-rotating-velocity-branch.md) condition

$$
\boxed{\left(\mu_1-e\frac{\mu_3}{d_4}\right)
[\mu_2^2+(\omega_2-\omega_3)^2]
=2c_2\mu_2\frac{\mu_3}{d_4}.}
$$

For $\mu_2^2+\Delta^2\ne0$, the zero-mode relation is $u+iv=-c_2s_0b/(\mu_2+i\Delta)$, so a nonzero $b$ gives a nonzero $A$ when $c_2\ne0$. With a transverse [eigenvalue](../../../../../eigenvalue.md) crossing and nondegenerate nonlinear saturation this is the generic magnetic bifurcation surface; magnetic reversal pairs its two signs. Degenerate cases require separate treatment. For example, if $\mu_2=\Delta=0$ and $c_2\ne0$, determinant zero is automatic but the stationary $u$ equation forces $b=0$, so that zero mode does not establish the requested branch with both magnetic amplitudes nonzero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
