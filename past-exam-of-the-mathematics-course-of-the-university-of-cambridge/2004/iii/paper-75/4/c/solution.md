<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $h_0=h_1(0)$ and $\rho_{10}=\rho_1(0)$, and write $\rho_L(t)$ for the mixed lower-layer density. Put

$$
D(t)=\frac{g}{\rho_{\rm ref}}h_1(t)[\rho_L(t)-\rho_2],\quad D_0=\frac{g}{\rho_{\rm ref}}h_0(\rho_{10}-\rho_2),\quad P=\frac{fB_0}{A},\quad K=\frac{4\pi\alpha^3}{3},\quad C=\sqrt{\frac{B_0}{2K}}.
$$

Use the common Boussinesq reference/inertial density normalization from part (a). Here $A D$ is the integrated negative buoyancy of the lower layer relative to the upper one. Assume negligible source volume, fixed enclosure volume, small density contrasts, identical thermals with total buoyancy $B_0$, slow evolution during one rise, and deposition of their positive buoyancy in the lower layer until penetration begins. Entrainment of upper fluid carries zero density anomaly relative to $\rho_2$, while thermal injection reduces the negative anomaly. The lower-layer [conservation of mass](../../../../../../mass-conservation.md) or equivalent buoyancy budget is therefore

$$
\boxed{D(t)=D_0-Pt,\qquad \rho_L(t)=\rho_2+\frac{\rho_{\rm ref}}g\frac{D_0-Pt}{h_1(t)}}.
$$

It would be inconsistent to conserve $h_1(\rho_L-\rho_2)$ while also depositing the nonzero source buoyancy $fB_0$.

Quasi-steady [point-source spherical thermal similarity](../../../../../../point-source-spherical-thermal-similarity.md) at the interface gives $b^*=\alpha h_1$ and $u^*=C/h_1$. The [Richardson number](../../../../../../richardson-number.md) compares the potential-energy barrier associated with the density jump to the thermal's available kinetic energy:

$$
\mathrm{Ri}=\frac{g'b^*}{u^{*2}}=\frac{\alpha D(t)h_1^2}{C^2}.
$$

An entrainment coefficient $c$ must be positive for upward deepening. A positive exponent $n$ makes stronger stratification inhibit entrainment; $n=0$ removes this dependence and $n<0$ would perversely strengthen entrainment as the stabilizing barrier increases. The power law is intended for a suitable finite-$\mathrm{Ri}$ regime: as $\mathrm{Ri}\to0$, its divergence must be limited by available turbulent motion. Its constants and validity are closure information, not consequences of dimensions alone. An additional kinetic-energy constraint is useful: the interfacial lifting cost scales as $\rho_0g'b^*Eu^*$, while the impinging turbulent power scales as $\rho_0u^{*3}$. Hence $E\mathrm{Ri}=c\mathrm{Ri}^{1-n}$ must remain of order one or smaller. A law intended to hold at arbitrarily large $\mathrm{Ri}$ with no extra power source therefore requires $n\geq1$; for $n=1$, $c$ measures a bounded conversion efficiency up to geometric factors. The requested $c=1$ represents an ideal order-one efficiency in this normalization.

For $c=n=1$, use the printed closure as a cycle-averaged interface law. Then

$$
\frac{dh_1}{dt}=\frac{u^{*3}}{g'b^*}=\frac{C^3}{\alpha[D_0-Pt]h_1^3}.
$$

Integrating from $h_0$ gives the [thermal erosion of a two-layer interface](../../../../../../thermal-erosion-of-a-two-layer-interface.md) result

$$
\boxed{h_1(t)=\left[h_0^4-\frac{4C^3}{\alpha P}\ln\left(1-\frac{Pt}{D_0}\right)\right]^{1/4}},\qquad 0<t<t^*,\quad Pt<D_0.
$$

The thermal's density deficit relative to the lower layer at height $h_1$ is $\rho_{\rm ref}B_0/(gKh_1^3)$. Under the question's buoyancy-controlled penetration criterion, the threshold thermal is neutral relative to the upper layer. Hence

$$
D(t^*)h_*^2=\frac{B_0}{K},\qquad h_*=h_1(t^*),\qquad \boxed{\rho_L(t^*)=\rho_2+\frac{\rho_{\rm ref}B_0}{gKh_*^3}}.
$$

The time and height are determined implicitly by this threshold and the explicit $h_1(t)$ law. Equivalently,

$$
\left[\frac{B_0}{K(D_0-Pt^*)}\right]^2=h_0^4-\frac{4C^3}{\alpha P}\ln\left(1-\frac{Pt^*}{D_0}\right).
$$

Use its first admissible root, provided it occurs before the upper layer is exhausted. Impingement initially requires $B_0<KD_0h_0^2$; otherwise penetration is immediate in this criterion. Depending on parameters, $D(t)h_1(t)^2$ can initially increase as entrainment deepens the layer, but it ultimately decreases to zero, so the first downward threshold crossing selects $t^*$.

The printed $E=\dot h_1/u^*$ must be an already averaged law to use it for separated thermal arrivals; if $c$ describes only an isolated impingement, an encounter duration/area averaging factor is missing and the same numerical formula cannot be asserted. The present answer uses the supplied averaged closure. It also uses the natural inherited $B_0$ per thermal; neglecting deposition of source buoyancy would instead give the different no-source-budget approximation $h_1^4=h_0^4+4C^3t/(\alpha D_0)$. The two budgets are explicitly distinguished. Real inertial penetration can precede neutral buoyancy, but that requires an additional head/penetration model absent here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
