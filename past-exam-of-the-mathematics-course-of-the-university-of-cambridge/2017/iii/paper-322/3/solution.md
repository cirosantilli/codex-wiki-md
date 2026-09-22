<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Set $\mathbf r=\mathbf x_1-\mathbf x_2$, $M=M_1+M_2$ and $\mu=M_1M_2/M$, the [reduced mass](../../../../../reduced-mass.md). [Newton's law of universal gravitation](../../../../../newton-s-law-of-universal-gravitation.md) gives $\ddot{\mathbf x}_1=-GM_2\mathbf r/r^3$ and $\ddot{\mathbf x}_2=GM_1\mathbf r/r^3$. Subtraction establishes

$$
\boxed{\ddot{\mathbf r}=-\frac{GM}{r^3}\mathbf r.}
$$

For fixed masses, the orbital [energy](../../../../../energy.md) and [angular momentum](../../../../../angular-momentum.md) are

$$
E=\frac{\mu}{2}\mathbf v^2-\frac{GM\mu}{r},\qquad \mathbf J=\mu\mathbf r\times\mathbf v,\qquad \mathbf v=\dot{\mathbf r}.
$$

Taking derivatives gives $\dot E=\mu\mathbf v\cdot(\ddot{\mathbf r}+GM\mathbf r/r^3)=0$ and $\dot{\mathbf J}=\mu\mathbf r\times\ddot{\mathbf r}=0$. These are [conservation of energy](../../../../../conservation-of-energy.md) and [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) in the unperturbed [Kepler orbit](../../../../../kepler-orbit.md). To see directly that the [orbital eccentricity](../../../../../orbital-eccentricity.md) is fixed, put $\mathbf h=\mathbf r\times\mathbf v$ and $\mathbf n=\mathbf r/r$. The [eccentricity vector](../../../../../eccentricity-vector.md) is

$$
\mathbf e=\frac{\mathbf v\times\mathbf h}{GM}-\mathbf n.
$$

Since $\dot{\mathbf h}=0$, the [cross product](../../../../../cross-product.md) identity $\mathbf r\times(\mathbf r\times\mathbf v)=\mathbf r(\mathbf r\cdot\mathbf v)-r^2\mathbf v$ gives $\ddot{\mathbf r}\times\mathbf h=GM\dot{\mathbf n}$, so $\dot{\mathbf e}=0$. Its magnitude $e$ is the [orbital eccentricity](../../../../../orbital-eccentricity.md). Equivalently,

$$
\boxed{e^2=1+\frac{2EJ^2}{G^2M^2\mu^3},\qquad E=-\frac{GM\mu}{2a}.}
$$

Thus the [semi-major axis](../../../../../semi-major-axis.md) and [orbital eccentricity](../../../../../orbital-eccentricity.md) of a bound noncollision [Kepler orbit](../../../../../kepler-orbit.md) are constant, including $e=0$.

Take the [centre of mass](../../../../../center-of-mass.md) as origin. The two positions are $\mathbf x_1=(M_2/M)\mathbf r$ and $\mathbf x_2=-(M_1/M)\mathbf r$. For $x\gg r$, a [Taylor expansion](../../../../../taylor-expansion.md) gives

$$
\frac1{|\mathbf x-\mathbf b|}=\frac1x+\frac{\mathbf x\cdot\mathbf b}{x^3}+\frac{3(\mathbf x\cdot\mathbf b)^2-x^2b^2}{2x^5}+O\left(\frac{b^3}{x^4}\right).
$$

The mass dipole vanishes because $\sum_A M_A\mathbf x_A=0$, and the [second mass moment tensor](../../../../../second-mass-moment-tensor.md) is $\sum_A M_Ax_{Ai}x_{Aj}=\mu r_i r_j$. The [gravitational quadrupole potential of a point-mass binary](../../../../../gravitational-quadrupole-potential-of-a-point-mass-binary.md) is consequently

$$
\Phi(\mathbf x)=-\frac{GM}{x}-\frac{G\mu}{2x^5}\bigl[3(\mathbf x\cdot\mathbf r)^2-x^2r^2\bigr]+O\left(\frac{GMr^3}{x^4}\right).
$$

Both printed tensors are trace-free. Contracting them with the [Kronecker delta](../../../../../kronecker-delta.md) summed over three spatial dimensions gives

$$
q_{ij}l_{ij}=\frac{\mu}{2x^5}\bigl[3(\mathbf x\cdot\mathbf r)^2-x^2r^2\bigr].
$$

This proves the requested expression through second order. In particular the printed convention is $q_{ij}=\tfrac32 Q_{ij}$, where $Q_{ij}=\mu(r_ir_j-r^2\delta_{ij}/3)$ is the standard [mass quadrupole moment](../../../../../mass-quadrupole-moment.md); the radiation coefficient must be adjusted accordingly. No mass dipole term may be retained in [centre of mass](../../../../../center-of-mass.md) coordinates.

To evaluate the [quadrupole formula](../../../../../quadrupole-formula.md) without assuming a [circular orbit](../../../../../circular-orbit.md), put $k=GM$, $u=\dot r=\mathbf n\cdot\mathbf v$ and $\mathbf v_\perp=\mathbf v-u\mathbf n$. Differentiating the [gravitational acceleration](../../../../../gravitational-acceleration.md) gives the [kinematic jerk](../../../../../jerk-kinematics.md)

$$
\dddot{\mathbf r}=-\frac{k}{r^3}(\mathbf v-3u\mathbf n).
$$

For $S_{ij}=r_ir_j$, the product rule then gives

$$
\dddot S_{ij}=\frac{k}{r^2}\bigl[-4(n_iv_j+v_in_j)+6u n_i n_j\bigr],\qquad \frac{d^3r^2}{dt^3}=-\frac{2ku}{r^2}.
$$

Inserting these into the printed [mass quadrupole moment](../../../../../mass-quadrupole-moment.md) convention yields

$$
\dddot q_{ij}=\frac{\mu k}{r^2}\bigl[u(\delta_{ij}-3n_in_j)-6(n_iv_{\perp j}+v_{\perp i}n_j)\bigr].
$$

The two tensors in brackets are orthogonal in their [tensor contraction](../../../../../tensor-contraction.md), because $\mathbf n\cdot\mathbf v_\perp=0$. Their squared norms are $6$ and $2v_\perp^2$, respectively. Hence

$$
\dddot q_{ij}\dddot q_{ij}=\frac{\mu^2k^2}{r^4}(6u^2+72v_\perp^2)=\frac{72\mu^2k^2}{r^4}\left(\mathbf v^2-\frac{11}{12}u^2\right).
$$

The [instantaneous quadrupole luminosity of a Kepler binary](../../../../../instantaneous-quadrupole-luminosity-of-a-kepler-binary.md) is therefore

$$
\boxed{\dot E=-\frac{32G^3M^2\mu^2}{5c^5r^4}\left(\dot{\mathbf r}\cdot\dot{\mathbf r}-\frac{11}{12}\dot r^2\right).}
$$

The radial derivative $\dot r$ is not the vector speed. The bracket equals $v_\perp^2+u^2/12$, so the radiated [luminosity](../../../../../luminosity.md) is nonnegative for every instantaneous velocity.

For a slowly evolving [circular orbit](../../../../../circular-orbit.md), there is no preferred orbital phase at which to excite a persistent [eccentricity vector](../../../../../eccentricity-vector.md). More precisely, the rotating [mass quadrupole moment](../../../../../mass-quadrupole-moment.md) emits at twice the orbital frequency, with angular harmonic number two; its [gravitational-wave energy and angular-momentum balance](../../../../../gravitational-wave-energy-and-angular-momentum-balance.md) is $\dot E=\Omega\dot J$. The circular [Kepler orbit](../../../../../kepler-orbit.md) sequence has $J=\mu\sqrt{GMa}$ and $dE/dJ=\Omega$, so this loss is tangent to the sequence. At leading adiabatic order it preserves zero secular [orbital eccentricity](../../../../../orbital-eccentricity.md). This is a [circular gravitational-wave inspiral](../../../../../circular-gravitational-wave-inspiral.md), with a small radial drift rather than an exactly fixed-radius Newtonian circle. The [energy](../../../../../energy.md) flux alone would not establish circularity without this symmetry and [angular momentum](../../../../../angular-momentum.md) balance.

To leading radiation order use $r=a$, $u=0$ and $\mathbf v^2=GM/a$ in the loss formula. Combining it with $E=-GM\mu/(2a)$ gives

$$
\frac{GM\mu}{2a^2}\dot a=-\frac{32G^4M^3\mu^2}{5c^5a^5},\qquad
\boxed{\frac{\dot a}{a}=-\frac{64G^3M^2\mu}{5c^5a^4}.}
$$

Keeping the fixed masses and leading [quadrupole formula](../../../../../quadrupole-formula.md), integration gives

$$
a(t)^4=a_0^4-\frac{256G^3M^2\mu}{5c^5}(t-t_0),\qquad
\boxed{t_{\rm coal}-t_0=\frac{5c^5a_0^4}{256G^3M^2\mu}.}
$$

This formal coalescence time displays the strong $a_0^4$ dependence: [gravitational-wave emission from a binary system](../../../../../gravitational-wave-emission-from-a-binary-system.md) matters far more for close [binary stars](../../../../../binary-star.md) than for wide ones. The [orbital period](../../../../../orbital-period.md) decreases as $a^{3/2}$ and the [gravitational-wave frequency](../../../../../gravitational-wave-frequency.md) increases, producing a chirp. A [detached binary](../../../../../detached-binary.md) can be driven into [Roche-lobe overflow](../../../../../roche-lobe-overflow.md); further evolution then depends on mass-transfer stability. A sufficiently close compact pair may merge. The weak-field, slow-motion, point-mass approximation ceases to apply before literal $a=0$; finite stellar radii or strong relativistic effects determine the final interaction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
