# Turbulent plume

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turbulent_plume)

A turbulent plume is a buoyancy-driven shear flow that grows by entraining ambient fluid.

**Table of contents**

- [Lazy plume](#lazy-plume)
- [Filling box model](#filling-box-model)
  - [Finite-source filling-box front with a side opening](#finite-source-filling-box-front-with-a-side-opening)
  - [Filling-box first front](#filling-box-first-front)
    - [Symmetric line-plume filling-box front](#symmetric-line-plume-filling-box-front)
- [Forced plume](#forced-plume)
  - [Jet length](#jet-length)
  - [Inclined forced plume](#inclined-forced-plume)
    - [Horizontal forced-plume trajectory](#horizontal-forced-plume-trajectory)
- [Buoyancy flux](#buoyancy-flux)
- [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis)
  - [Entrainment coefficient](#entrainment-coefficient)
- [Top-hat plume model](#top-hat-plume-model)
  - [Confined plume with compensating return flow](#confined-plume-with-compensating-return-flow)
    - [Confined-plume momentum fold](#confined-plume-momentum-fold)
  - [Source-volume length of a turbulent plume](#source-volume-length-of-a-turbulent-plume)
  - [Jet limit of the top-hat plume model](#jet-limit-of-the-top-hat-plume-model)
  - [Weak hyperbolicity of the unsteady top-hat plume](#weak-hyperbolicity-of-the-unsteady-top-hat-plume)
  - [Unsteady top-hat line-plume balances](#unsteady-top-hat-line-plume-balances)
    - [Separable decaying top-hat line plume](#separable-decaying-top-hat-line-plume)
  - [Merger of two equal pure plumes](#merger-of-two-equal-pure-plumes)
    - [Fixed-speed pure-plume merger and flux conservation](#fixed-speed-pure-plume-merger-and-flux-conservation)
  - [Boussinesq top-hat plume in a stratified ambient](#boussinesq-top-hat-plume-in-a-stratified-ambient)
    - [Plume similarity in power-law stratification](#plume-similarity-in-power-law-stratification)
      - [Top-hat plume in constant unstable stratification](#top-hat-plume-in-constant-unstable-stratification)
      - [Amplitudes and physical branches of a power-law stratified plume](#amplitudes-and-physical-branches-of-a-power-law-stratified-plume)
      - [Logarithmic-height plume equations](#logarithmic-height-plume-equations)
        - [Growing mode of power-law plume similarity](#growing-mode-of-power-law-plume-similarity)
  - [Kinematic plume fluxes](#kinematic-plume-fluxes)
  - [Non-Boussinesq top-hat plume equations](#non-boussinesq-top-hat-plume-equations)
    - [Non-Boussinesq pure-plume density transition](#non-boussinesq-pure-plume-density-transition)
  - [Pure plume](#pure-plume)
    - [Pure plume balance](#pure-plume-balance)
      - [Plume flux-balance invariant](#plume-flux-balance-invariant)
        - [Finite-source forced-plume quadrature](#finite-source-forced-plume-quadrature)
        - [Attraction to pure plume similarity](#attraction-to-pure-plume-similarity)
      - [Plume balance parameter](#plume-balance-parameter)
    - [Axisymmetric pure plume](#axisymmetric-pure-plume)
      - [Radius growth of an axisymmetric pure plume](#radius-growth-of-an-axisymmetric-pure-plume)
      - [Neutral buoyancy-flux mode of a pure plume](#neutral-buoyancy-flux-mode-of-a-pure-plume)
      - [Boussinesq point-source plume](#boussinesq-point-source-plume)
    - [Line plume](#line-plume)
      - [Triangular-profile line plume](#triangular-profile-line-plume)
        - [Unsteady Boussinesq triangular-profile line-plume balances](#unsteady-boussinesq-triangular-profile-line-plume-balances)
          - [Separable decaying line-plume similarity](#separable-decaying-line-plume-similarity)
        - [Non-Boussinesq triangular-profile line-plume balances](#non-boussinesq-triangular-profile-line-plume-balances)
      - [Two-sided top-hat line plume](#two-sided-top-hat-line-plume)
      - [Wall line plume](#wall-line-plume)
        - [Melting-driven saline wall plume](#melting-driven-saline-wall-plume)
        - [Ice-bearing wall-plume thermodynamic invariant](#ice-bearing-wall-plume-thermodynamic-invariant)
          - [Self-similar ice-bearing wall plume](#self-similar-ice-bearing-wall-plume)
        - [Triangular-profile wall line plume](#triangular-profile-wall-line-plume)
      - [Stratified line-plume height scale](#stratified-line-plume-height-scale)
    - [Plume virtual origin](#plume-virtual-origin)
      - [Forced-plume virtual-origin geometry](#forced-plume-virtual-origin-geometry)
- [Heated wall plume](#heated-wall-plume)
- [Buoyant thermal](#buoyant-thermal)
  - [Thermal erosion of a two-layer interface](#thermal-erosion-of-a-two-layer-interface)
  - [Point-source spherical thermal similarity](#point-source-spherical-thermal-similarity)
  - [Dilute bubbly thermal](#dilute-bubbly-thermal)
    - [Neutral height of a bubbly thermal in a stratified fluid](#neutral-height-of-a-bubbly-thermal-in-a-stratified-fluid)
  - [Buoyant thermal mass balance](#buoyant-thermal-mass-balance)
- [Starting plume](#starting-plume)
  - [Self-similar starting plume](#self-similar-starting-plume)
    - [Starting-plume thermal Froude-number ratio](#starting-plume-thermal-froude-number-ratio)
- [Buoyant intrusion](#buoyant-intrusion)

## Lazy plume

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A buoyant plume with insufficient momentum for the corresponding [pure plume balance](#pure-plume-balance). In the constant-entrainment top-hat model it has [plume balance parameter](#plume-balance-parameter) $\Gamma>1$, unlike the momentum-excess [forced plume](#forced-plume). The equations accelerate the plume and drive the balance parameter toward one downstream. The definition depends on the chosen flux and [entrainment](fluid-mechanics.md#fluid-entrainment) convention; it is not merely a synonym for slow vertical speed.

## Filling box model

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A filling box model describes a [turbulent plume](turbulent-plume.md) rising through a confined fluid and spreading beneath its ceiling. [Fluid entrainment](fluid-mechanics.md#fluid-entrainment) transfers initially unmodified ambient fluid into the plume; the discharged fluid forms a descending [filling-box first front](#filling-box-first-front). A maintained heat source can have negligible source [volume flux](fluid-mechanics.md#volumetric-flow-rate) while maintaining nonzero [buoyancy flux](#buoyancy-flux). A finite injected fluid flux requires an equal exhaust if the container volume is fixed.

### Finite-source filling-box front with a side opening

↑ **Parent:** [Filling box model](#filling-box-model)

For a source in [pure plume balance](#pure-plume-balance), $Q(z)=C F_s^{1/3}(z+z_v)^{5/3}$ and $Q_s=Q(0)$. A single ideal exhaust passes the source volume flux. Above the exhaust height, it removes unprocessed lower fluid and the [filling-box first front](#filling-box-first-front) descends at rate $-\pi Q/A_c$. Below it, processed fluid leaves and only entrained volume grows the processed region. The floor is reached in finite time if the opening is at the floor; otherwise the final approach is exponential. A finite-height aperture supporting bidirectional exchange requires a different model.

### Filling-box first front

↑ **Parent:** [Filling box model](#filling-box-model)

In a [filling box model](#filling-box-model), the first front separates fluid already modified by plume discharge from the initially unmodified fluid below. If the plume occupies a negligible fraction of horizontal area $A$, its [volume flux](fluid-mechanics.md#volumetric-flow-rate) across the front is $P(h)$, and the ceiling exhaust is $F$, [volume conservation](physics.md#volume-conservation) gives $A\dot h=F-P(h)$. For a closed box with a negligible-volume buoyancy source, $F=0$. For a finite injected source flux $Q$ with ceiling overflow $Q$, $F=Q$. The first front need not delimit a uniformly mixed upper layer throughout the unventilated transient.

#### Symmetric line-plume filling-box front

↑ **Parent:** [Filling-box first front](#filling-box-first-front)

An ideal two-sided [line plume](#line-plume) has half-width $b=\alpha z$, constant [velocity](classical-mechanics.md#velocity) $w_*=(\mathcal B/(2\alpha))^{1/3}$ and [volume flux](fluid-mechanics.md#volumetric-flow-rate) $q=2\alpha w_*z$. In a closed box of width $2R$, neglecting the plume's occupied area gives $2R\dot h=-q(h)$ for the [filling-box first front](#filling-box-first-front), initially at ceiling height $H$. With negligible diffusion the front is a material interface; its ambient [buoyancy](fluid-mechanics.md#buoyancy) jump retains the initial ceiling-discharge value $\mathcal B/q(H)=w_*^2/H$. The contemporaneous plume [reduced gravity](reduced-gravity.md) $w_*^2/h(t)$ is a different quantity. The upper ambient generally becomes stratified rather than remaining one uniformly mixed layer.

## Forced plume

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A forced plume has both imposed [momentum flux](physics.md#momentum-flux) and positive [buoyancy flux](#buoyancy-flux). Its near-source region behaves like a jet, while its far field approaches a [pure plume](#pure-plume). The crossover is measured by a [jet length](#jet-length).

### Jet length

↑ **Parent:** [Forced plume](#forced-plume)

For source kinematic [momentum flux](physics.md#momentum-flux) $m_0$ and [buoyancy flux](#buoyancy-flux) $f_0>0$, [dimensional analysis](physics.md#dimensional-analysis) gives $L_J=m_0^{3/4}/f_0^{1/2}$. Under constant [Batchelor entrainment](#batchelor-entrainment-hypothesis), the actual turning length also contains an [entrainment coefficient](#entrainment-coefficient) factor of order $\alpha^{-1/2}$.

### Inclined forced plume

↑ **Parent:** [Forced plume](#forced-plume)

An inclined [forced plume](#forced-plume) curves upward under [buoyancy](fluid-mechanics.md#buoyancy). In a stationary homogeneous ambient, its horizontal [momentum flux](physics.md#momentum-flux) is conserved and its vertical [momentum flux](physics.md#momentum-flux) increases. For [kinematic plume fluxes](#kinematic-plume-fluxes), $m_x'=0$ and $m_z'=fq/m$, where $m=\sqrt{m_x^2+m_z^2}$ and the derivative is with respect to centreline [arc length](riemannian-geometry.md#arc-length).

#### Horizontal forced-plume trajectory

↑ **Parent:** [Inclined forced plume](#inclined-forced-plume)

For zero source [volume flux](fluid-mechanics.md#volumetric-flow-rate), constant [Batchelor entrainment](#batchelor-entrainment-hypothesis), and a horizontal source, the near-source trajectory is cubic: $z\sim\alpha\sqrt{\pi}f_0x^3/(3m_0^{3/2})$. Far from the source the centreline approaches a vertical asymptote, with its horizontal distance from that asymptote proportional to $z^{-1/3}$.

## Buoyancy flux

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

The buoyancy flux through a section is the integral of velocity times reduced gravity. In a Boussinesq pure plume in a uniform ambient it is conserved.

## Batchelor entrainment hypothesis

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

The [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis) takes the inward mean edge velocity of a [turbulent plume](turbulent-plume.md) to be $v_e=\alpha w$ in the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation). Its density-corrected non-Boussinesq form is $v_e=\alpha w\sqrt{\rho/\rho_0}$, where $\rho$ and $\rho_0$ are plume and ambient [mass densities](fluid-mechanics.md#density) and $\alpha$ is the [entrainment coefficient](#entrainment-coefficient).

### Entrainment coefficient

↑ **Parent:** [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis)

The entrainment coefficient is the dimensionless constant in the [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis), so the mean speed at which ambient fluid crosses a plume edge is $\alpha$ times the plume's characteristic axial speed.

## Top-hat plume model

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A top-hat plume model takes velocity and reduced gravity to be uniform across the plume and zero outside it. Integral volume, momentum, and [buoyancy fluxes](#buoyancy-flux) then depend only on plume width and these uniform values.

### Confined plume with compensating return flow

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

In an impermeable cylinder, an axisymmetric [turbulent plume](turbulent-plume.md) with negligible source [volume flux](fluid-mechanics.md#volumetric-flow-rate) requires a downward return flow. With uniform upward plume [velocity](classical-mechanics.md#velocity) $w$ and ambient [velocity](classical-mechanics.md#velocity) $v$, [volume conservation](physics.md#volume-conservation) gives $b^2w+(R^2-b^2)v=0$. An [entrainment coefficient](#entrainment-coefficient) $\alpha$ based on the relative speed gives $Q'=2\alpha b(w-v)$. A specified pressure closure is essential for [momentum conservation](classical-mechanics.md#momentum-conservation). If the departure from ambient [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) and wall force are neglected in the whole-section integral, the total specific [momentum flux](physics.md#momentum-flux) $J=b^2w^2+(R^2-b^2)v^2$ obeys $J'=b^2g'$. Homogeneous unmodified ambient and no buoyancy loss give $b^2wg'=B_s$. These are leading integral-model closures; restoring the ambient dynamic pressure can change the singularity criterion.

#### Confined-plume momentum fold

↑ **Parent:** [Confined plume with compensating return flow](#confined-plume-with-compensating-return-flow)

For the pressure-neglecting [confined plume with compensating return flow](#confined-plume-with-compensating-return-flow), define specific plume [momentum flux](physics.md#momentum-flux) $M=b^2w^2$ and area fraction $s=Q^2/(R^2M)$. Then $J=M/(1-s)$ and

$$
(1-2s)M'=\frac{B_sQ}{M}(1-s)^2-\frac{2Q}{R^2}Q'.
$$

The branch issuing from a [pure plume](#pure-plume) reaches a fold at $s=1/2$, where plume and ambient have equal areas, opposite [velocities](classical-mechanics.md#velocity) and equal specific [momentum fluxes](physics.md#momentum-flux). The numerator is nonzero on this branch, so $M'$ diverges although $M,Q,w$ remain finite. This signals failure of the steady uniform-profile description, not infinite physical velocity.

### Source-volume length of a turbulent plume

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

Source [volume flux](fluid-mechanics.md#volumetric-flow-rate) is negligible only when entrained volume greatly exceeds it. In the [jet limit of the top-hat plume model](#jet-limit-of-the-top-hat-plume-model), this requires $z\gg Q_0/(c\sqrt{M_0})$. In a [pure plume](#pure-plume) with $Q=C_Qz^{5/3}$, it requires $z\gg(Q_0/C_Q)^{3/5}$, where $C_Q=(3c/5)(9cF_0/20)^{1/3}$ for full-cross-section fluxes and $c=2\alpha_e\sqrt\pi$. These scales differ from the [jet length](#jet-length) which measures imposed momentum relative to buoyancy. Neglecting source volume does not automatically permit neglecting source momentum.

### Jet limit of the top-hat plume model

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

With zero source [volume flux](fluid-mechanics.md#volumetric-flow-rate) and zero [buoyancy flux](#buoyancy-flux) but positive source [momentum flux](physics.md#momentum-flux), the axisymmetric [top-hat plume model](#top-hat-plume-model) reduces to a turbulent round jet. For full-cross-section kinematic fluxes, put $c=2\alpha_e\sqrt\pi$. [Entrainment](fluid-mechanics.md#fluid-entrainment) gives $Q'=c\sqrt M$, while momentum conservation gives $M=M_0$. Hence $Q=c\sqrt{M_0}z$, speed $w=\sqrt{M_0}/(cz)$ and radius $r=cz/\sqrt\pi$. A finite source flux replaces $z$ by $z+Q_0/(c\sqrt{M_0})$. The ideal zero-flux source has singular speed and is a far-field model, not a finite nozzle.

### Weak hyperbolicity of the unsteady top-hat plume

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

For plume area $A$ and reduced gravity $g'$, the principal matrix in variables $(A,w,g')$ is $\begin{pmatrix}w&A&0\\0&w&0\\0&0&w\end{pmatrix}$. At $A>0$ it has a triple real speed $w$ but only two independent eigenvectors. Thus the model is weakly hyperbolic, not strongly or strictly hyperbolic. Real speeds alone do not provide a complete set of characteristic fields or a uniform high-frequency estimate. Shape factors representing nonuniform radial profiles can alter this degeneracy.

### Unsteady top-hat line-plume balances

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

Use half-width $b$, upward speed $w$, constant inertial reference density $R$, and positive buoyant [reduced gravity](reduced-gravity.md) $g'$. Half-section fluxes are $Q=Rbw$, $M=Rbw^2$ and $F=Rg'bw$. With two-sided [entrainment](fluid-mechanics.md#fluid-entrainment) $u_e=\alpha w$, the [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) balances are

$$
(Q^2/M)_t+Q_z=R\alpha M/Q,\qquad
Q_t+M_z=FQ/M,\qquad
(FQ/M)_t+F_z=-N^2Q.
$$

Full-width fluxes are twice these definitions. The shape coefficients differ from triangular transverse profiles, so their unsteady balances cannot be used unchanged here.

#### Separable decaying top-hat line plume

↑ **Parent:** [Unsteady top-hat line-plume balances](#unsteady-top-hat-line-plume-balances)

In a homogeneous ambient fluid, the displayed nonsteady [power-law ansatz](differential-equation.md#power-law-ansatz) solves the [unsteady top-hat line-plume balances](#unsteady-top-hat-line-plume-balances) for $\tau=t+t_*>0$. It gives $Q=R\alpha z^2/(3\tau)$, $M=2R\alpha z^3/(9\tau^2)$ and $F=2R\alpha z^3/(9\tau^3)$. The solution is singular at zero age and carries zero source flux at its unshifted ideal origin. It describes a separable branch away from a source; a finite-width boundary, virtual-origin shift or matching region is needed to supply nonzero physical source flux. It is distinct from the steady constant-flux line plume, whose top-hat half-width grows as $\alpha z$.

### Merger of two equal pure plumes

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

If two equal [pure plumes](#pure-plume) merge while keeping their common velocity and [reduced gravity](reduced-gravity.md), conservation of cross-sectional area gives radius $\sqrt2$ times the individual radius. All three integral fluxes double. The [plume balance parameter](#plume-balance-parameter) increases by $2^3/2^{5/2}=\sqrt2$, so the immediate combined plume is a [lazy plume](#lazy-plume). Similarity attraction may restore pure balance farther downstream, but instantaneous pure balance does not follow from adding two [pure plumes](#pure-plume).

#### Fixed-speed pure-plume merger and flux conservation

↑ **Parent:** [Merger of two equal pure plumes](#merger-of-two-equal-pure-plumes)

For a merged pair held at the original velocity and [reduced gravity](reduced-gravity.md), [pure plume balance](#pure-plume-balance) requires the original individual radius, not the larger area-preserving radius. The required pure area is half the combined area. Shrinking to that area at unchanged velocity and [reduced gravity](reduced-gravity.md) would halve volume, momentum and [buoyancy fluxes](#buoyancy-flux), contradicting conservation of the merged fluxes. A conservative merger must change its properties or begin away from pure balance.

### Boussinesq top-hat plume in a stratified ambient

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

With common factors of $\pi$ removed, steady kinematic fluxes satisfy $Q_z=2\alpha\sqrt M$, $M_z=FQ/M$ and $F_z=-N^2Q$. The [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis) supplies volume, the integrated [buoyancy](fluid-mechanics.md#buoyancy) force supplies momentum, and the environmental [mass density](fluid-mechanics.md#density) gradient reduces [buoyancy flux](#buoyancy-flux). This uses the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation).

#### Plume similarity in power-law stratification

↑ **Parent:** [Boussinesq top-hat plume in a stratified ambient](#boussinesq-top-hat-plume-in-a-stratified-ambient)

For $N^2=Kz^\beta$ and positive pure-power fluxes, the [similarity solution](partial-differential-equation.md#similarity-solution) exponents are $q=3+\beta/2$, $m=4+\beta$ and $f=4+3\beta/2$. Increasing volume and momentum and decreasing positive [buoyancy flux](#buoyancy-flux) require $-4<\beta<-8/3$. At fixed nonzero $K$ the endpoint coefficient limits are singular.

##### Top-hat plume in constant unstable stratification

↑ **Parent:** [Plume similarity in power-law stratification](#plume-similarity-in-power-law-stratification)

For prescribed $N^2=-G^2<0$, the steady [Boussinesq top-hat plume in a stratified ambient](#boussinesq-top-hat-plume-in-a-stratified-ambient) has kinematic fluxes $Q=\alpha^2Gz^3/9$, $M=\alpha^2G^2z^4/36$, and $F=\alpha^2G^3z^4/36$. Balancing powers in $Q_z=2\alpha\sqrt M$, $M_z=FQ/M$, and $F_z=G^2Q$ gives exponents $(3,4,4)$ and these positive amplitudes. The ambient's static instability is prescribed without allowing it to drive ambient motion; the Boussinesq approximation additionally requires small density differences over the modeled height range.

##### Amplitudes and physical branches of a power-law stratified plume

↑ **Parent:** [Plume similarity in power-law stratification](#plume-similarity-in-power-law-stratification)

For the [Boussinesq top-hat plume in a stratified ambient](#boussinesq-top-hat-plume-in-a-stratified-ambient) with $N^2=Cz^p$, the exact pure-power solution has the displayed radius and velocity, and $g'=-2Cz^{p+1}/(3p+8)$. With positive entrainment, radius, upward speed and reduced gravity, stable $C>0$ requires $-4<p<-8/3$, whereas unstable $C<0$ requires $p>-8/3$. The stable branch has divergent buoyancy flux at zero height, so it is not a finite-flux point-source solution. The unstable branch has zero limiting source buoyancy flux and extracts buoyancy from its maintained unstable ambient. The cases $p=-6,-4,-8/3$ are singular at nonzero $C$; $C=0$ instead admits the ordinary [Boussinesq point-source plume](#boussinesq-point-source-plume).

##### Logarithmic-height plume equations

↑ **Parent:** [Plume similarity in power-law stratification](#plume-similarity-in-power-law-stratification)

Normalize volume, momentum and buoyancy by a positive [plume similarity in power-law stratification](#plume-similarity-in-power-law-stratification) and use $\xi=\ln(z/z_*)$. The normalized equations are $\widehat Q_\xi=q(\sqrt{\widehat M}-\widehat Q)$, $\widehat M_\xi=m(\widehat F\widehat Q/\widehat M-\widehat M)$ and $\widehat F_\xi=f(\widehat Q-\widehat F)$. They form an [autonomous differential equation](dynamical-systems.md#autonomous-system-mathematics).

###### Growing mode of power-law plume similarity

↑ **Parent:** [Logarithmic-height plume equations](#logarithmic-height-plume-equations)

The linearized relative-flux matrix is $J=[(-q,q/2,0);(m,-2m,m);(f,0,-f)]$. Its [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) has constant term $qmf<0$ for physical positive-buoyancy similarity, so at least one real [eigenvalue](linear-operator-theory.md#eigenvalue) is positive. The growing mode behaves as $z^\lambda$ and makes the similarity trajectory unstable with increasing height, rather than with physical time.

### Kinematic plume fluxes

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

Dividing the [mass flux](physics.md#mass-flux), [momentum flux](physics.md#momentum-flux), and density-weighted [buoyancy flux](#buoyancy-flux) by ambient [mass density](fluid-mechanics.md#density) gives the kinematic fluxes $q=\pi b^2V$, $m=\pi b^2V^2$, and $f=\pi b^2Vg(\rho_0-\rho)/\rho_0$. This convention makes dimensional [similarity solutions](partial-differential-equation.md#similarity-solution) independent of the arbitrary ambient density unit.

### Non-Boussinesq top-hat plume equations

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

For a [turbulent plume](turbulent-plume.md) in a homogeneous ambient of density $\rho_0$, define actual sectional [mass flux](physics.md#mass-flux), [momentum flux](physics.md#momentum-flux) and density-weighted [buoyancy flux](#buoyancy-flux) by $Q=\pi b^2\rho w$, $M=\pi b^2\rho w^2$ and $F=\pi b^2wg(\rho_0-\rho)$. With non-Boussinesq [Batchelor entrainment](#batchelor-entrainment-hypothesis) $v_e=\alpha w\sqrt{\rho/\rho_0}$, their balances are

$$
\partial_t(Q^2/M)+\partial_zQ=2\alpha\sqrt{\pi\rho_0M},\qquad
\partial_tQ+\partial_zM=QF/M,\qquad
\partial_t(QF/M)+\partial_zF=0.
$$

Here $Q^2/M$ is sectional mass, $QF/M$ is sectional density-deficit buoyancy, and the entrained ambient initially has zero vertical momentum. The last equation follows by subtracting mass conservation from $\rho_0$ times volume conservation. [Scase, Caulfield, Dalziel and Hunt's time-dependent plume model](https://doi.org/10.1017/S0022112006001212) derives the equivalent system with the common factor $\pi$ suppressed.

#### Non-Boussinesq pure-plume density transition

↑ **Parent:** [Non-Boussinesq top-hat plume equations](#non-boussinesq-top-hat-plume-equations)

For an ideal-gas heated [pure plume](#pure-plume) with entrainment proportional to $w\sqrt{\rho/\rho_0}$, the excess heat flux implies conserved kinematic buoyancy flux $B$. Put $q=Q/\rho_0$, $m=M/\rho_0$. Their balances are $q'=2\alpha\sqrt m$ and $m'=Bq/m$, identical to the pi-suppressed Boussinesq pure-plume flux equations. With $d=6\alpha/5$ and $s=[25B/(48\alpha^2)]^{1/3}$, $q=d^2s z^{5/3}$, $m=d^2s^2z^{4/3}$ and $z_b^{5/3}=B/(gd^2s)$. The radius is $b=dz\sqrt{1+(z_b/z)^{5/3}}$ and reduced gravity is $g/[1+(z/z_b)^{5/3}]$. At $z=z_b$ density is half ambient; far above this height the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) becomes accurate.

### Pure plume

↑ **Parent:** [Top-hat plume model](#top-hat-plume-model)

A pure plume is a similarity regime in which the source supplies [buoyancy flux](#buoyancy-flux) but no dynamically persistent source volume or momentum flux. Its finite source region is represented by a [plume virtual origin](#plume-virtual-origin).

#### Pure plume balance

↑ **Parent:** [Pure plume](#pure-plume)

For the constant-entrainment axisymmetric plume equations $Q'=2\alpha\sqrt M$, $M'=FQ/M$ with $F>0$, pure balance means $M^{5/2}=5FQ^2/(8\alpha)$ at every height. This is a similarity relation between fluxes, not a requirement that the physical source have zero radius. A finite source on this curve is represented by a [plume virtual origin](#plume-virtual-origin). For fluxes normalized by pi and top-hat fields, the same relation is $g'b/w^2=8\alpha/5$.

##### Plume flux-balance invariant

↑ **Parent:** [Pure plume balance](#pure-plume-balance)

When $F$ and $\alpha$ are constant, eliminating height between $Q'=2\alpha\sqrt M$ and $M'=FQ/M$ gives $d(M^{5/2})/dQ=5FQ/(4\alpha)$. Thus $M^{5/2}-5FQ^2/(8\alpha)$ is constant. Its sign classifies forced and lazy departures from [pure plume balance](#pure-plume-balance), and its vanishing makes a finite-source plume exactly self-similar after a virtual-origin shift.

###### Finite-source forced-plume quadrature

↑ **Parent:** [Plume flux-balance invariant](#plume-flux-balance-invariant)

For an axisymmetric [top-hat plume model](#top-hat-plume-model) in uniform ambient density, use full kinematic fluxes and $c=2\alpha_e\sqrt\pi$. The equations $Q'=c\sqrt M$, $M'=F_0Q/M$ conserve $M^{5/2}-5F_0Q^2/(4c)$. Solve this invariant for $M(Q)$, then integrate $dz=dQ/(c\sqrt M)$ to obtain the displayed exact quadrature. It determines the transition from the near-source [jet limit of the top-hat plume model](#jet-limit-of-the-top-hat-plume-model) to the distant [pure plume](#pure-plume). The two regimes cannot be added by linear superposition because the flux equations are nonlinear.

###### Attraction to pure plume similarity

↑ **Parent:** [Plume flux-balance invariant](#plume-flux-balance-invariant)

For positive source fluxes and positive constant [buoyancy flux](#buoyancy-flux), the [plume flux-balance invariant](#plume-flux-balance-invariant) has a finite constant while $Q$ grows without bound. Dividing by $Q^2$ makes the source imbalance vanish relatively. The balances then give $Q\sim(6\alpha/5)(9\alpha F/10)^{1/3}z^{5/3}$ and $M\sim(9\alpha F/10)^{2/3}z^{4/3}$. This attraction concerns relative similarity and does not assert that different finite sources share the same virtual origin.

##### Plume balance parameter

↑ **Parent:** [Pure plume balance](#pure-plume-balance)

The dimensionless ratio $\Gamma=5FQ^2/(8\alpha M^{5/2})$ compares a plume to the constant-entrainment pure balance. Values one, below one and above one describe [pure plume balance](#pure-plume-balance), a momentum-excess [forced plume](#forced-plume), and a momentum-deficient [lazy plume](#lazy-plume), respectively. For fluxes normalized by pi and a top-hat profile, $\Gamma=5g'b/(8\alpha w^2)$.

#### Axisymmetric pure plume

↑ **Parent:** [Pure plume](#pure-plume)

For a top-hat axisymmetric pure plume of radius $r$, speed $U$, and reduced gravity $g'$, the conserved fluxes are $Q=\pi r^2U$, $M=\pi r^2U^2$, and $B=\pi r^2Ug'$. The [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis) gives $Q\propto B^{1/3}z^{5/3}$.

##### Radius growth of an axisymmetric pure plume

↑ **Parent:** [Axisymmetric pure plume](#axisymmetric-pure-plume)

For pi-normalized top-hat fluxes, $b=Q/\sqrt M$. The pure [similarity solution](partial-differential-equation.md#similarity-solution) therefore has $b=(6\alpha/5)(z+z_0)$, so the radius grows linearly with slope $6\alpha/5$. The corresponding [plume virtual origin](#plume-virtual-origin) is $-z_0$ and a finite source has $z_0=5b_s/(6\alpha)$. This law translates geometric plume-contact criteria into heights.

##### Neutral buoyancy-flux mode of a pure plume

↑ **Parent:** [Axisymmetric pure plume](#axisymmetric-pure-plume)

A constant surviving [buoyancy flux](#buoyancy-flux) sets the amplitudes of a [pure plume](#pure-plume): $Q\propto F^{1/3}$ and $M\propto F^{2/3}$. Relative-flux perturbations have the neutral ratio $(\delta Q/Q,\delta M/M,\delta F/F)\propto(1,2,3)$. This is the zero-eigenvalue limit of [growing mode of power-law plume similarity](#growing-mode-of-power-law-plume-similarity); nonzero endpoint stratification can still create cumulative logarithmic flux loss.

##### Boussinesq point-source plume

↑ **Parent:** [Axisymmetric pure plume](#axisymmetric-pure-plume)

A steady [top-hat plume model](#top-hat-plume-model) supplied with kinematic [buoyancy flux](#buoyancy-flux) $f_0>0$ but zero source [volume flux](fluid-mechanics.md#volumetric-flow-rate) and [momentum flux](physics.md#momentum-flux) has

$$
b=az,\qquad w=Kz^{-1/3},\qquad g'=\frac43K^2z^{-5/3},\qquad
a=\frac{6\alpha}{5},\quad K^3=\frac{25f_0}{48\alpha^2}.
$$

The [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis) and momentum balance yield these constants. Its [Froude number](reduced-gravity.md#froude-number) satisfies $w^2/(g'b)=5/(8\alpha)$. The [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) requires $g'/g\ll1$ and therefore fails at the ideal point source itself.

#### Line plume

↑ **Parent:** [Pure plume](#pure-plume)

A line plume is invariant along one horizontal direction, so its integral fluxes are measured per unit span. A wall line plume entrains through one exposed edge and has width proportional to distance from its [plume virtual origin](#plume-virtual-origin).

##### Triangular-profile line plume

↑ **Parent:** [Line plume](#line-plume)

A two-sided [line plume](#line-plume) whose axial [velocity](classical-mechanics.md#velocity) and density anomaly both have triangular transverse profiles. For half-width $b$, $\int_{-b}^bf(x/b)^n\,dx=2b/(n+1)$. These profile moments set the different coefficients of stored [mass](classical-mechanics.md#mass), [momentum](classical-mechanics.md#momentum), and their fluxes. It differs from a wall plume because both edges entrain ambient fluid.

###### Unsteady Boussinesq triangular-profile line-plume balances

↑ **Parent:** [Triangular-profile line plume](#triangular-profile-line-plume)

In the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), density-weighted fluxes are $Q=\rho_0bW$, $M=(2/3)\rho_0bW^2$ and $F=(2/3)gbW(\rho_0-\rho)$. With two-sided [Batchelor entrainment](#batchelor-entrainment-hypothesis) $e=\alpha W$, the integral balances are

$$
\frac43(Q^2/M)_t+Q_z=3\alpha\rho_0M/Q,\qquad Q_t+M_z=FQ/M,\qquad(FQ/M)_t+F_z=0.
$$

The factors $4/3$ and $3$ depend on the triangular profile and the definition of the [entrainment coefficient](#entrainment-coefficient).

###### Separable decaying line-plume similarity

↑ **Parent:** [Unsteady Boussinesq triangular-profile line-plume balances](#unsteady-boussinesq-triangular-profile-line-plume-balances)

The [unsteady Boussinesq triangular-profile line-plume balances](#unsteady-boussinesq-triangular-profile-line-plume-balances) admit a buoyant [similarity solution](partial-differential-equation.md#similarity-solution) $Q=\alpha\rho_0z^2/\tau$, $M=(2/3)\alpha\rho_0z^3/\tau^2$ and $F=(2/3)\alpha\rho_0z^3/\tau^3$, with $\tau=t+t_*>0$. It reconstructs $b=\alpha z$, $W=z/\tau$ and reduced gravity $z/\tau^2$. Origins can be shifted, but the zero-time unshifted solution is singular. Source and initial data are required to select the physical member and region of validity.

###### Non-Boussinesq triangular-profile line-plume balances

↑ **Parent:** [Triangular-profile line plume](#triangular-profile-line-plume)

For a [triangular-profile line plume](#triangular-profile-line-plume) with centreline density $\rho$, speed $W$, half-width $b$, ambient density $\rho_0$, and inward relative edge speed $e$, [volume](geometry-and-topology.md#volume), [mass](classical-mechanics.md#mass) and [momentum](classical-mechanics.md#momentum) conservation give

$$
(2b)_t+(bW)_z=2e,\quad [b(\rho+\rho_0)]_t+[bW(\rho_0+2\rho)/3]_z=2\rho_0e,
$$



$$
[bW(\rho_0+2\rho)/3]_t+[bW^2(\rho_0+3\rho)/6]_z=gb(\rho_0-\rho).
$$

Subtracting [mass conservation](continuum-mechanics.md#mass-conservation) from $\rho_0$ times [volume](geometry-and-topology.md#volume) conservation also gives buoyancy conservation. [Batchelor entrainment](#batchelor-entrainment-hypothesis) supplies a closure for $e$.

##### Two-sided top-hat line plume

↑ **Parent:** [Line plume](#line-plume)

For a [top-hat plume model](#top-hat-plume-model) with full width $w$, upward speed $U$, [reduced gravity](reduced-gravity.md) $b$, and edge [entrainment coefficient](#entrainment-coefficient) $e$, define [volume flux](fluid-mechanics.md#volumetric-flow-rate) per unit span $V=wU$, kinematic [momentum flux](physics.md#momentum-flux) $M=wU^2$, and [buoyancy flux](#buoyancy-flux) $B=wUb$. A uniform ambient and two exposed edges give $V'=2eU$, $M'=wb=B/U$, and $B'=0$. A [pure plume](#pure-plume) with $V(0)=0$ has

$$
U=\left(\frac B{2e}\right)^{1/3},\qquad w=2ez,\qquad V=(2e)^{2/3}B^{1/3}z.
$$

Indeed $M=UV$ with constant $U$ reduces the momentum balance to $2eU^3=B$. If width means half-width, its growth coefficient is $e$, not $2e$; profile shape factors also alter the coefficients.

##### Wall line plume

↑ **Parent:** [Line plume](#line-plume)

A wall line plume is a one-sided [line plume](#line-plume) adjoining a solid wall. Under a top-hat pure-plume model, $d(bW)/ds=\alpha W$ because only its outer edge entrains ambient fluid.

###### Melting-driven saline wall plume

↑ **Parent:** [Wall line plume](#wall-line-plume)

A glacier supplies fresh meltwater at speed $U>0$ to a rising [wall line plume](#wall-line-plume) whose buoyancy is dominated by [salinity](physics.md#salinity). With one entraining edge, [entrainment coefficient](#entrainment-coefficient) $\varepsilon$, [volume flux](fluid-mechanics.md#volumetric-flow-rate) $Q=bw$ and negligible wall stress, $Q'=\varepsilon w+U$ and $(bw^2)'=g\beta_C(C_\infty-C)b$. Enthalpy and salt balances give $[Q(T_\infty-T)]'=U[L/c_p+T_\infty-T_s]$ and $[Q(C_\infty-C)]'=U(C_\infty-C_s)$. If latent heat dominates and entrainment dominates the volume supply, integration from a virtual origin $Z=0$ and power-law balance give the displayed width and speed. The temperature and salinity deficits are $ULZ/(c_pQ)$ and $U(C_\infty-C_s)Z/Q$, both proportional to $Z^{-1/3}$. The approximation is a far-field plume solution, not a solution at the virtual origin.

###### Ice-bearing wall-plume thermodynamic invariant

↑ **Parent:** [Wall line plume](#wall-line-plume)

An ice-bearing plume at local liquidus equilibrium conserves excess enthalpy $E$ and salt $S$ relative to the ambient liquidus water. Eliminating its temperature and brine composition gives $\phi Q[L+c_pmC_0-L\phi]=-E-c_pmS+E\phi$. To dilute-crystal order this fixes its advected ice volume, hence its leading buoyancy flux. A positive rising branch needs a positive source invariant.

###### Self-similar ice-bearing wall plume

↑ **Parent:** [Ice-bearing wall-plume thermodynamic invariant](#ice-bearing-wall-plume-thermodynamic-invariant)

For one exposed entraining edge and conserved positive dilute ice flux $I_0$, the line-plume equations give the displayed pure far-field solution. Its width grows linearly, speed is constant and ice fraction decays inversely with distance from a virtual origin. Two exposed edges replace $e$ by $2e$. The dilute solution is invalid near the formal origin, where its ice fraction diverges.

###### Triangular-profile wall line plume

↑ **Parent:** [Wall line plume](#wall-line-plume)

In a triangular-profile wall line plume, axial velocity and [reduced gravity](reduced-gravity.md) decrease linearly from their wall values to zero across the plume width $b$. If the wall speed is $W$, its volume and kinematic momentum fluxes per unit span are $V=bW/2$ and $J=bW^2/3$.

##### Stratified line-plume height scale

↑ **Parent:** [Line plume](#line-plume)

A line plume of kinematic [buoyancy flux](#buoyancy-flux) $B_0$ rising through uniform [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$ has the dimensional height scale

$$
z_s=\frac{B_0^{1/3}}N.
$$

It measures the height over which ambient stratification removes an order-one fraction of the plume buoyancy before the plume reaches neutral buoyancy and spreads as a [buoyant intrusion](#buoyant-intrusion).

#### Plume virtual origin

↑ **Parent:** [Pure plume](#pure-plume)

A plume virtual origin is the extrapolated point at which a similarity plume's width and volume flux vanish. It absorbs finite source geometry into a shift of the axial coordinate.

##### Forced-plume virtual-origin geometry

↑ **Parent:** [Plume virtual origin](#plume-virtual-origin)

For a horizontal [forced plume](#forced-plume), the [plume virtual origin](#plume-virtual-origin) lies downstream and below the physical source on the far-field vertical asymptote. The origin shift in centreline [arc length](riemannian-geometry.md#arc-length) is distinct from its vertical height: if $z=s-D+o(1)$ and $\hat s=s+s_0$, the virtual height is $z_v=-D-s_0$. Both geometric shifts scale with the [jet length](#jet-length) at fixed [entrainment coefficient](#entrainment-coefficient).

## Heated wall plume

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A heated wall plume is a one-sided plume adjacent to a wall. A uniform wall heat flux makes its buoyancy flux grow linearly with height.

## Buoyant thermal

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A buoyant thermal is a localized rising volume of fluid whose [mass density](fluid-mechanics.md#density) is lower than its surroundings. It can form the head of a [starting plume](#starting-plume). A spherical mixed thermal of radius $R$ has volume $V=4\pi R^3/3$ and [reduced gravity](reduced-gravity.md) $g_t=g(\rho_0-\rho_t)/\rho_0$ in the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation).

### Thermal erosion of a two-layer interface

↑ **Parent:** [Buoyant thermal](#buoyant-thermal)

Suppose identical [buoyant thermals](#buoyant-thermal) deliver buoyancy $B_0$ at rate $f$ to a mixed lower layer of area $A$ before penetrating its interface. Neglect source volume and heat loss. Relative to the upper-layer density, let $D=g h(\rho_L-\rho_2)/\rho_{\rm ref}$, $P=fB_0/A$, and $C=\sqrt{B_0/(2K)}$, where $K=4\pi\alpha^3/3$. The lower-layer buoyancy budget gives $D=D_0-Pt$. A cycle-averaged [fluid entrainment](fluid-mechanics.md#fluid-entrainment) closure $\dot h/u^*=\mathrm{Ri}^{-1}$, with $u^*=C/h$, $b^*=\alpha h$, yields the displayed law. Neutrality of the thermal at the interface requires $D(t^*)h(t^*)^2=B_0/K$. The closure must incorporate the encounter duty cycle; an isolated-event entrainment law needs an additional averaging prescription.

### Point-source spherical thermal similarity

↑ **Parent:** [Buoyant thermal](#buoyant-thermal)

In the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), a spherical [buoyant thermal](#buoyant-thermal) with conserved total buoyancy $B_0$ obeys $\dot b=\alpha u$ and $d(Vu)/dt=B_0$, with $V=4\pi b^3/3$. A zero-volume, zero-impulse point source gives $b=\alpha z$, $Kz^3\dot z=B_0t$, where $K=4\pi\alpha^3/3$. Hence $z^4=2B_0t^2/K$ and $u=\sqrt{B_0/(2K)}/z$. The zero-time singularity represents an ideal source limit, not a finite initially regular sphere.

### Dilute bubbly thermal

↑ **Parent:** [Buoyant thermal](#buoyant-thermal)

A dilute bubbly thermal is a rising, entraining fluid volume whose gas bubbles provide part of its [buoyancy](fluid-mechanics.md#buoyancy). With negligible bubble slip and gas loss, [Boyle's law](thermodynamics.md#boyle-s-law) gives gas volume proportional to $(1-z/H_p)^{-1}$, where $H_p=p_0/(\rho_0g)$. Spherical [fluid entrainment](fluid-mechanics.md#fluid-entrainment) with normal entrainment velocity $\alpha W$ gives $da/dz=\alpha$. Bubble concentration follows by dividing the gas volume by the growing thermal volume. A diameter-based [Froude number](reduced-gravity.md#froude-number) closure is $W=F\sqrt{2ag'}$.

#### Neutral height of a bubbly thermal in a stratified fluid

↑ **Parent:** [Dilute bubbly thermal](#dilute-bubbly-thermal)

For a constant ambient [buoyancy frequency](gravity-wave.md#buoyancy-frequency), entrained liquid lags the decreasing ambient density by $\rho_0N^2[(a_0+\alpha z)^4-a_0^4]/[4\alpha g(a_0+\alpha z)^3]$. Balancing this negative buoyancy with expanding-bubble buoyancy gives the displayed fifth-degree equation. The first physically admissible root is the neutral height in the quasi-steady rise-speed model. In a very deep release, bubble expansion is negligible and $z_n=[(a_0^4+4\alpha g\phi_0a_0^3/N^2)^{1/4}-a_0]/\alpha$. Actual momentum can cause overshoot, while bubble slip becomes important as the liquid stops rising.

### Buoyant thermal mass balance

↑ **Parent:** [Buoyant thermal](#buoyant-thermal)

If a [buoyant thermal](#buoyant-thermal) receives volume inflow $J$ with [reduced gravity](reduced-gravity.md) $g_p$ and receives no other [fluid entrainment](fluid-mechanics.md#fluid-entrainment), its mass and volume balances imply $\dot V=J$ and $d(g_tV)/dt=g_pJ$. If $V\propto t^{9/4}$ and $g_t\propto t^{-5/4}$, then $g_t=9g_p/4$.

## Starting plume

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A starting plume is the unsteady flow formed when a maintained [buoyancy flux](#buoyancy-flux) first begins. An idealized model joins a steady [pure plume](#pure-plume) below its growing head to a [buoyant thermal](#buoyant-thermal) above. [Turner's original starting-plume study](https://doi.org/10.1017/S0022112062000762) develops this plume-and-thermal description.

### Self-similar starting plume

↑ **Parent:** [Starting plume](#starting-plume)

For constant kinematic [buoyancy flux](#buoyancy-flux) $f_0$ from a point source, [dimensional analysis](physics.md#dimensional-analysis) gives head height and radius proportional to $f_0^{1/4}t^{3/4}$, head velocity proportional to $f_0^{1/4}t^{-1/4}$, and head [reduced gravity](reduced-gravity.md) proportional to $f_0^{1/4}t^{-5/4}$. Dimensionless coefficients require the chosen [fluid entrainment](fluid-mechanics.md#fluid-entrainment) and head closures.

#### Starting-plume thermal Froude-number ratio

↑ **Parent:** [Self-similar starting plume](#self-similar-starting-plume)

For a spherical [buoyant thermal](#buoyant-thermal) fed only through the moving top of a [Boussinesq point-source plume](#boussinesq-point-source-plume), put $\lambda=R/B$ and $B=(6\alpha/5)Z$. Relative inflow $\pi B^2(w_p-\dot Z)$ and $\dot V=4\pi R^2\dot R$ imply

$$
\frac{\dot Z}{w_p}=\frac5{5+24\alpha\lambda^3}.
$$

The ratio of [Froude numbers](reduced-gravity.md#froude-number) is $5/[\sqrt\lambda(5+24\alpha\lambda^3)]$ when both use plume [reduced gravity](reduced-gravity.md) $g_p$. Normalizing the thermal with its own $g_t=9g_p/4$ multiplies this by $2/3$. These two definitions must not be interchanged when stating bounds.

## Buoyant intrusion

↑ **Parent:** [Turbulent plume](turbulent-plume.md)

A buoyant intrusion is a predominantly horizontal current formed when a rising or sinking plume reaches nearly neutral buoyancy in a stratified ambient fluid. The plume's momentum generally carries it beyond its neutral-buoyancy level before it spreads.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (14)

- [Batchelor entrainment hypothesis](#batchelor-entrainment-hypothesis)
- [Confined plume with compensating return flow](#confined-plume-with-compensating-return-flow)
- [Filling box model](#filling-box-model)
- [Non-Boussinesq top-hat plume equations](#non-boussinesq-top-hat-plume-equations)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-80.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330.md#2/b/solution)
- [Turbulence](turbulence.md)
