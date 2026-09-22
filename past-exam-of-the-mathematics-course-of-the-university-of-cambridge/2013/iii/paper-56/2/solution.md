<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $\mathbf r=\mathbf x_1-\mathbf x_2$, $r=|\mathbf r|$ and $M=M_1+M_2$. [Newton's law of universal gravitation](../../../../../newton-s-law-of-universal-gravitation.md) gives $\ddot{\mathbf x}_1=-GM_2\mathbf r/r^3$ and $\ddot{\mathbf x}_2=GM_1\mathbf r/r^3$. Subtracting yields the **relative two-body equation**

$$
\boxed{\ddot{\mathbf r}=-\frac{GM}{r^3}\mathbf r.}
$$

The [reduced mass](../../../../../reduced-mass.md) is $\mu=M_1M_2/M$. The orbital energy and [angular momentum](../../../../../angular-momentum.md) in the [center of mass](../../../../../center-of-mass.md) frame are

$$
E=\frac\mu2|\dot{\mathbf r}|^2-\frac{GM\mu}{r},\qquad
\mathbf J=\mu\mathbf r\times\dot{\mathbf r}.
$$

Differentiation gives

$$
\dot E=\mu\dot{\mathbf r}\cdot\ddot{\mathbf r}+\frac{GM\mu}{r^3}\mathbf r\cdot\dot{\mathbf r}=0,
\qquad
\dot{\mathbf J}=\mu\mathbf r\times\ddot{\mathbf r}=0.
$$

Thus both are conserved. The [eccentricity vector](../../../../../eccentricity-vector.md) is

$$
\mathbf e=\frac{\dot{\mathbf r}\times(\mathbf r\times\dot{\mathbf r})}{GM}-\frac{\mathbf r}{r}.
$$

For $\mathbf h=\mathbf J/\mu$, one has $\ddot{\mathbf r}\times\mathbf h/(GM)=\dot{\mathbf r}/r-\mathbf r(\mathbf r\cdot\dot{\mathbf r})/r^3=d(\mathbf r/r)/dt$, so $\dot{\mathbf e}=0$. In particular the **[orbital eccentricity](../../../../../orbital-eccentricity.md) is constant**, with

$$
\boxed{e^2=1+\frac{2EJ^2}{G^2M^2\mu^3}.}
$$

For a bound [Kepler orbit](../../../../../kepler-orbit.md), $E=-GM\mu/(2a)$ and $J^2=GM\mu^2a(1-e^2)$.

For the far-field [multipole expansion](../../../../../electric-multipole-expansion.md), set the [center of mass](../../../../../center-of-mass.md) to zero. Then $\mathbf x_1=(M_2/M)\mathbf r$ and $\mathbf x_2=-(M_1/M)\mathbf r$. At $x=|\mathbf x|\gg r$, expand each point-mass [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md):

$$
\frac1{|\mathbf x-\mathbf x_A|}=\frac1x+\frac{x_i x_{Ai}}{x^3}
+\frac12x_{Ai}x_{Aj}\frac{3x_ix_j-x^2\delta_{ij}}{x^5}+O(r^3/x^4).
$$

Repeated indices are summed. The dipole vanishes since $\sum_A M_A\mathbf x_A=0$, and $\sum_A M_Ax_{Ai}x_{Aj}=\mu r_ir_j$. The second-order [gravitational quadrupole potential of a point-mass binary](../../../../../gravitational-quadrupole-potential-of-a-point-mass-binary.md) is therefore

$$
\phi(\mathbf x)=-\frac{GM}{x}-\frac{G\mu}{2x^5}\left[3(\mathbf x\cdot\mathbf r)^2-x^2r^2\right]+O(GMr^3/x^4).
$$

Both tensors specified in the question are trace-free. Direct contraction gives

$$
q_{ij}l_{ij}=\frac{\mu}{2x^5}\left[3(\mathbf x\cdot\mathbf r)^2-x^2r^2\right],
$$

so **to the requested order**

$$
\boxed{\phi(\mathbf x)=-\frac{GM}{x}-Gq_{ij}l_{ij}(\mathbf x).}
$$

For equal masses the cubic multipole also vanishes, but it need not vanish for unequal masses.

To evaluate the [quadrupole formula](../../../../../quadrupole-formula.md), use $k=GM$, $\mathbf v=\dot{\mathbf r}$, $\mathbf n=\mathbf r/r$, $u=\dot r=\mathbf n\cdot\mathbf v$, and $\mathbf w=\mathbf v-u\mathbf n$. The acceleration and its derivative are

$$
\mathbf b=-\frac{k\mathbf n}{r^2},\qquad
\dot{\mathbf b}=-\frac{k\mathbf v}{r^3}+\frac{3ku\mathbf n}{r^3}.
$$

The third derivative of $r_ir_j$ is $\dot b_i r_j+r_i\dot b_j+3b_i v_j+3v_i b_j$. Its trace is $d^3(r^2)/dt^3=-2ku/r^2$. Substituting in $q_{ij}=\mu(3r_ir_j-r^2\delta_{ij})/2$ gives

$$
\frac{d^3q_{ij}}{dt^3}=\frac{\mu k}{r^2}\left[u(\delta_{ij}-3n_in_j)-6(n_iw_j+w_in_j)\right].
$$

Because $\mathbf n\cdot\mathbf w=0$, the cross [tensor contraction](../../../../../tensor-contraction.md) is zero. The squared norms of the two bracketed pieces are $6u^2$ and $72w^2$, respectively. Thus

$$
\dddot q_{ij}\dddot q_{ij}=\frac{72\mu^2k^2}{r^4}\left(v^2-\frac{11}{12}u^2\right),
$$

and the **instantaneous energy loss** is

$$
\boxed{\dot E=-\frac{32G^3M^2\mu^2}{5c^5r^4}\left(\dot{\mathbf r}\cdot\dot{\mathbf r}-\frac{11}{12}\dot r^2\right).}
$$

The parenthesis is $w^2+u^2/12\geq0$, as required for positive radiated power. This is the [instantaneous quadrupole luminosity of a Kepler binary](../../../../../instantaneous-quadrupole-luminosity-of-a-kepler-binary.md) with loss sign for the orbital energy.

A slowly evolving initially circular binary is expected to follow a quasi-circular inspiral at leading radiation order. One needs angular-momentum loss as well as energy loss for this conclusion: the rotating quadrupole has frequency $2\Omega$ and azimuthal harmonic number two, so its fluxes satisfy the [gravitational-wave energy and angular-momentum balance](../../../../../gravitational-wave-energy-and-angular-momentum-balance.md) $\dot E=\Omega\dot J$. Along the circular family,

$$
E=-\frac{G^2M^2\mu^3}{2J^2},\qquad\frac{dE}{dJ}=\Omega.
$$

The flux relation is precisely the tangent condition for remaining on that family; equivalently it keeps $e^2=1+2EJ^2/(G^2M^2\mu^3)$ equal to zero at leading secular order. The shrinking orbit is not an exact fixed-radius circle: its small radial drift is neglected at this adiabatic order.

For a circular orbit of instantaneous separation $a$, $u=0$ and $v^2=GM/a$. Therefore

$$
\dot E=-\frac{32G^4M^3\mu^2}{5c^5a^5}.
$$

Differentiating $E=-GM\mu/(2a)$ at fixed masses now gives

$$
\boxed{\frac{\dot a}{a}=-\frac{64G^3M^2\mu}{5c^5a^4}.}
$$

Writing $C=64G^3M^2\mu/(5c^5)$, the [circular gravitational-wave inspiral](../../../../../circular-gravitational-wave-inspiral.md) obeys $a^4=a_0^4-4Ct$. The formal point-mass coalescence time is $a_0^4/(4C)$, and $\dot P/P=(3/2)\dot a/a$ gives a decreasing [orbital period](../../../../../orbital-period.md) and increasing [gravitational-wave frequency](../../../../../gravitational-wave-frequency.md).

**Gravitational radiation tightens a detached close binary and becomes more effective at small separation.** It can bring a stellar donor into [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) or drive compact objects toward merger. Finite radii, tides and mass transfer can then alter the evolution; the fixed-mass inspiral law is not the entire evolution law once these matter. Near merger the weak-field, slow-motion [quadrupole formula](../../../../../quadrupole-formula.md) also ceases to be sufficient.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
