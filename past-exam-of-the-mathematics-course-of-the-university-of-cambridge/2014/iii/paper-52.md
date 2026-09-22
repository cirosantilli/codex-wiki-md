# Paper 52

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_52.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_52.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
    - [iv](#2/a/iv)
      - [Solution](#2/a/iv/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
    - [v](#3/b/v)
      - [Solution](#3/b/v/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use [geometrized units](../../../general-relativity.md#geometrized-units) and [metric signature](../../../topology.md#metric-signature) $(-+++)$, with $M>0$. In the exterior of [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime), put $f=1-2M/r$. The [Schwarzschild tortoise coordinate](../../../general-relativity.md#schwarzschild-tortoise-coordinate) satisfies

$$
\frac{dr_*}{dr}=f^{-1},\qquad r_*=r+2M\log\left|\frac r{2M}-1\right|.
$$

The [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) $u=t-r_*$ and $v=t+r_*$ then give $ds^2=-f\,du\,dv+r^2d\Omega^2$. The logarithmic divergence of $r_*$ suggests exponentiating these [null coordinates](../../../general-relativity.md#null-coordinate). In the right exterior define the [Kruskal–Szekeres coordinates](../../../general-relativity.md#kruskal-szekeres-coordinates)

$$
U=-e^{-u/(4M)},\qquad V=e^{v/(4M)}.
$$

Their product eliminates $t$:

$$
UV=-e^{r_*/(2M)}=\left(1-\frac r{2M}\right)e^{r/(2M)}.
$$

Since $du=-4M\,dU/U$ and $dv=4M\,dV/V$, the [Schwarzschild metric](../../../general-relativity.md#schwarzschild-spacetime) becomes

$$
\boxed{ds^2=-\frac{32M^3}{r}e^{-r/(2M)}\,dU\,dV+r^2d\Omega^2,\qquad UV=\left(1-\frac r{2M}\right)e^{r/(2M)}.}
$$

Here $r$ is an implicitly defined function of $UV$. The derivative of the right side with respect to $r$ is $-r e^{r/(2M)}/(4M^2)$, which is nonzero at $r=2M$. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) therefore makes $r(UV)$ smooth across that surface, and the coefficient of $dU\,dV$ tends to $-16M^2/e$. Thus the [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon) is a coordinate singularity of the original chart, while this [Lorentzian metric](../../../general-relativity.md#lorentzian-metric) remains regular there.

Extend the [Kruskal–Szekeres coordinates](../../../general-relativity.md#kruskal-szekeres-coordinates) to all real $U,V$ with $UV<1$. The signs give two exterior regions, $U<0<V$ and $V<0<U$, a future [black hole](../../../general-relativity.md#black-hole) region $U,V>0$, and a past [white hole](../../../general-relativity.md#white-hole) region $U,V<0$. The [event horizons](../../../general-relativity.md#event-horizon) are $U=0$ or $V=0$, intersecting at the [bifurcation surface](../../../general-relativity.md#bifurcation-surface). The boundary $UV=1$ has $r=0$ and is a genuine [Schwarzschild singularity](../../../general-relativity.md#schwarzschild-singularity), as the [Kretschmann scalar](../../../general-relativity.md#kretschmann-scalar) $48M^2/r^6$ diverges there.

Finally, $T=(V+U)/2$ and $X=(V-U)/2$ give $UV=T^2-X^2$ and a radial metric proportional to $-dT^2+dX^2$. Hence radial [null geodesics](../../../special-relativity.md#null-geodesic) have slopes $\pm1$, the [event horizons](../../../general-relativity.md#event-horizon) are $T=\pm X$, and the singular boundaries are $T^2-X^2=1$. **This constructs the maximal Kruskal extension**; a [black hole](../../../general-relativity.md#black-hole) produced by collapse need not contain the second exterior or the [white hole](../../../general-relativity.md#white-hole) of that eternal extension.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Start with the four-dimensional [Minkowski metric](../../../special-relativity.md#minkowski-metric) $ds^2=-dt^2+dr^2+r^2d\Omega^2$, where $r\geq0$. Choose an arbitrary length $L>0$, and use the [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) $u=t-r$, $v=t+r$. For the [Minkowski conformal compactification](../../../general-relativity.md#minkowski-conformal-compactification), set

$$
p=\arctan(u/L),\quad q=\arctan(v/L),\qquad T=p+q,\quad R=q-p.
$$

Both $p,q$ lie between $-\pi/2$ and $\pi/2$. Since $v\geq u$, we have $R\geq0$; the remaining inequalities are $|T|+R<\pi$. Moreover,

$$
r=\frac{L\sin R}{2\cos p\cos q},\qquad ds^2=\frac{L^2}{4\cos^2p\cos^2q}\left(-dT^2+dR^2+\sin^2R\,d\Omega^2\right).
$$

Multiply by the square of the [conformal factor](../../../general-relativity.md#conformal-factor) $\Omega_c=2\cos p\cos q/L$. The resulting metric is regular on the appropriate boundary pieces and preserves the [null directions](../../../special-relativity.md#null-directions). Suppressing the angular two-spheres gives a triangular [Penrose diagram](../../../general-relativity.md#penrose-diagram) with radial [null geodesics](../../../special-relativity.md#null-geodesic) at $45$ degrees.

The line $R=0$ is the ordinary timelike centre $r=0$. The upper sloping edge $T+R=\pi$ is [future null infinity](../../../general-relativity.md#future-null-infinity), reached with $v\to+\infty$ and finite $u$; the lower sloping edge $T-R=-\pi$ is [past null infinity](../../../general-relativity.md#past-null-infinity), reached with $u\to-\infty$ and finite $v$. The vertices $(T,R)=(\pi,0)$ and $(-\pi,0)$ are future and past [timelike infinity](../../../general-relativity.md#timelike-infinity), denoted $i^+$ and $i^-$. The vertex $(0,\pi)$ is [spacelike infinity](../../../general-relativity.md#spacelike-infinity), $i^0$. These are limiting endpoints in the [conformal completion](../../../general-relativity.md#conformal-completion), rather than ordinary physical events. In particular, finite diagram coordinates at [null infinity](../../../general-relativity.md#null-infinity) do not imply finite physical [affine parameter](../../../riemannian-geometry.md#affine-parameter).

**The four-dimensional radial diagram is the triangle $R\geq0$, $|T|+R\leq\pi$.** If one instead draws two-dimensional [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with a signed Cartesian spatial coordinate, the diagram is the full diamond. The centre is a boundary of the radial quotient, not a boundary of the physical four-dimensional [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime).

<a id="1/b/image-kruskal-extension-and-the-radial-minkowski-penrose-diagram"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52-conformal-diagrams.png)

**[Figure 1](#1/b/image-kruskal-extension-and-the-radial-minkowski-penrose-diagram). Kruskal extension and the radial Minkowski Penrose diagram**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The physical argument for the [Penrose inequality](../../../general-relativity.md#penrose-inequality) combines [weak cosmic censorship conjecture](../../../general-relativity.md#weak-cosmic-censorship-conjecture), the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition), and relaxation to a stationary [black hole](../../../general-relativity.md#black-hole). Work in [geometrized units](../../../general-relativity.md#geometrized-units). Let $M_f$ and $A_f$ be the final [Kerr black hole](../../../general-relativity.md#kerr-black-hole) mass and horizon area. Positive energy radiated to infinity gives $E_{\rm ADM}\geq M_f$, where $E_{\rm ADM}$ is the initial [ADM energy](../../../general-relativity.md#arnowitt-deser-misner-energy). For a [Kerr black hole](../../../general-relativity.md#kerr-black-hole) with $a_f=J_f/M_f$,

$$
A_f=8\pi M_f\left(M_f+\sqrt{M_f^2-a_f^2}\right)\leq16\pi M_f^2.
$$

If the initial [apparent horizon](../../../general-relativity.md#apparent-horizon) obeys the necessary [apparent-horizon area comparison](../../../general-relativity.md#apparent-horizon-area-comparison) with the enclosing [event horizon](../../../general-relativity.md#event-horizon), and [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem) applies during the evolution, then

$$
A_{\rm app}\leq A_{\rm EH,initial}\leq A_f\leq16\pi M_f^2\leq16\pi E_{\rm ADM}^2.
$$

Consequently the anticipated answer, under those additional hypotheses, is

$$
\boxed{E_{\rm ADM}\geq\sqrt{\frac{A_{\rm app}}{16\pi}}.}
$$

The bound is saturated by a nonrotating [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime) with no energy loss. Rotation or outgoing radiation makes the argument's inequalities stricter.

There is an essential qualification: inclusion inside an [event horizon](../../../general-relativity.md#event-horizon) does not by itself compare areas. An arbitrary [apparent horizon](../../../general-relativity.md#apparent-horizon) on general, non-time-symmetric initial data need not satisfy the displayed [apparent-horizon area comparison](../../../general-relativity.md#apparent-horizon-area-comparison); the unqualified version with its area is not universally true, even with the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition). On time-symmetric data the relevant outermost [minimal surface](../../../second-fundamental-form.md#minimal-surface) is an [outer area-minimizing surface](../../../second-fundamental-form.md#outer-area-minimizing-surface), as used in the [Riemannian Penrose inequality](../../../general-relativity.md#riemannian-penrose-inequality), with nonnegative [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). In more general formulations an appropriate enclosing-area quantity is needed. **The physical expectation is conditional on this area comparison**, as well as on censorship, predictability, settling, and the energy assumptions; the mere presence of a [trapped surface](../../../general-relativity.md#trapped-surface) does not supply every step.

## 2

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) is a smooth local family of [null geodesics](../../../special-relativity.md#null-geodesic), with one generator through each point of the region being described. Choose an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\lambda$ on each generator and write $U^a=dx^a/d\lambda$. Before a caustic, $U$ is a smooth, nonzero [null vector](../../../special-relativity.md#null-vector) field satisfying $U^aU_a=0$ and $U^b\nabla_bU^a=0$.

With $B^a{}_b=\nabla_bU^a$, compatibility of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) with the [metric](../../../topological-analysis.md#metric) gives

$$
U_aB^a{}_b=U_a\nabla_bU^a=\frac12\nabla_b(U^aU_a)=0.
$$

The [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) with [affine parameter](../../../riemannian-geometry.md#affine-parameter) gives the other contraction:

$$
B^a{}_bU^b=U^b\nabla_bU^a=0.
$$

Thus **both contractions vanish**. Nullness supplies the first identity, and affine parametrization supplies the second; a general nonaffine tangent would instead have $B^a{}_bU^b=\kappa U^a$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Choose a local transverse three-dimensional section of the [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) and a future unit [timelike vector](../../../general-relativity.md#timelike-vector) $T$ on it. Orient $U$ to the future and put $E=-U\cdot T>0$. On that section define a [parallel auxiliary null vector](../../../geodesic-congruence.md#parallel-auxiliary-null-vector) by the initial value

$$
N^a=\frac{T^a}{E}-\frac{U^a}{2E^2}.
$$

Since $T^2=-1$, $U^2=0$, and $U\cdot T=-E$, direct contraction gives $U\cdot N=-1$ and $N^2=-E^{-2}+E^{-2}=0$.

Extend $N$ along each generator by [parallel transport](../../../fiber-bundle.md#parallel-transport), solving $U^b\nabla_bN^a=0$ with those initial values. The [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) and compatibility of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) imply

$$
U\cdot\nabla(N^2)=0,\qquad U\cdot\nabla(U\cdot N)=0.
$$

Therefore **$N^2=0$, $U\cdot N=-1$, and $\nabla_U N=0$ hold throughout the local congruence**. Smooth initial data and the transport equation give a smooth field up to the breakdown of the congruence at caustics. An arbitrary pointwise choice of $T$ away from the initial section would not automatically have this transport property.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) annihilates both [null vectors](../../../special-relativity.md#null-vector): $P^a{}_bU^b=P^a{}_bN^b=0$, and satisfies $P^2=P$. Its image is the two-dimensional spacelike screen orthogonal to $U,N$. The screen metric is

$$
q_{ab}=g_{ab}+U_aN_b+N_aU_b.
$$

It is positive definite on that screen. Projecting both indices of $B_{ab}=\nabla_bU_a$ gives the [optical tensor](../../../geodesic-congruence.md#optical-tensor) $\widehat B_{ab}=P_a{}^cP_b{}^dB_{cd}$.

Define its three parts by

$$
\boxed{\theta=q^{ab}\widehat B_{ab},\qquad \omega_{ab}=\widehat B_{[ab]},\qquad \sigma_{ab}=\widehat B_{(ab)}-\frac12\theta q_{ab}.}
$$

Thus $\widehat B_{ab}=\tfrac12\theta q_{ab}+\sigma_{ab}+\omega_{ab}$. The [null expansion](../../../geodesic-congruence.md#null-expansion) $\theta$ is its trace and equals $d\log\mathcal A/d\lambda$ for the infinitesimal beam area $\mathcal A$. The [null shear](../../../geodesic-congruence.md#null-shear) $\sigma$ is symmetric and trace-free, measuring shape change at fixed first-order area. The [null twist](../../../geodesic-congruence.md#null-twist) $\omega$, also called rotation, is antisymmetric and measures failure of screen directions to remain hypersurface-orthogonal. In $D$ dimensions replace $1/2$ by $1/(D-2)$. Here and below expansion means the trace, rather than its average over the screen dimensions.

<h4 id="2/a/iv">iv</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/a/iv)

Locally write the [null hypersurface](../../../general-relativity.md#null-hypersurface) as $F=0$. Its generators are tangent to its raised normal, so on it $U_a=h\nabla_aF$ for a nonzero scalar $h$. The antisymmetric derivative is

$$
\nabla_{[b}U_{a]}=(\nabla_{[b}h)(\nabla_{a]}F),
$$

since the Hessian of $F$ is symmetric for the torsion-free [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). Each term contains $\nabla F$, which is proportional to $U$ and is killed by the [screen-space projector](../../../geodesic-congruence.md#screen-space-projector). Hence

$$
\boxed{\omega_{ab}=P_a{}^cP_b{}^d\nabla_{[d}U_{c]}=0.}
$$

This is the null version of hypersurface orthogonality in the [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem). A [null hypersurface](../../../general-relativity.md#null-hypersurface) has no independent normal direction outside its tangent space: its [null vector](../../../special-relativity.md#null-vector) normal also generates it. That is why the same argument applies to the generators' [null twist](../../../geodesic-congruence.md#null-twist).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

For the round sphere, every normal has only $v,r$ components because the [Reissner-Nordstrom metric](../../../general-relativity.md#reissner-nordstrom-spacetime) has no mixed angular terms. The vector $X=-\partial_r$ is normal and null: $g_{rr}=0$. Write the second [null vector](../../../special-relativity.md#null-vector) normal as $Y=A\partial_v+B\partial_r$. The normalization gives $X\cdot Y=-A=-1$, so $A=1$. Its [null condition](../../../special-relativity.md#null-condition) then reads $-f+2B=0$. Thus

$$
\boxed{X=-\partial_r,\qquad Y=\partial_v+\frac{f(r_0)}2\partial_r\quad\text{on }S.}
$$

The specified future orientation of $X$, together with $X\cdot Y<0$, makes $Y$ future-directed as well. This choice fixes the reciprocal scaling freedom of the two [null vectors](../../../special-relativity.md#null-vector) on the sphere.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For each of the two normal directions, launch a [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) orthogonally from the sphere with initial tangent $U=X$ or $U=Y$. For $U=X$ take initial auxiliary $N=Y$; for $U=Y$ take initial $N=X$, and then [parallel transport](../../../fiber-bundle.md#parallel-transport) $N$ as in part (a). On the sphere the resulting [screen-space projector](../../../geodesic-congruence.md#screen-space-projector) projects onto its angular tangent space, whose metric is $q_{AB}=r^2\gamma_{AB}$.

For any radial normal $K$, the [spherical null expansion in ingoing coordinates](../../../geodesic-congruence.md#spherical-null-expansion-in-ingoing-coordinates) follows directly from area variation:

$$
\theta_K=\frac12q^{AB}\mathcal L_Kq_{AB}=\frac{2K(r)}r.
$$

Equivalently $\mathcal A\propto r^2$ gives $K(\log\mathcal A)=2K(r)/r$. Consequently

$$
\boxed{\theta_X=-\frac2{r_0},\qquad \theta_Y=\frac{f(r_0)}{r_0}=\frac{(r_0-r_+)(r_0-r_-)}{r_0^3}.}
$$

Spherical symmetry also makes the [null shear](../../../geodesic-congruence.md#null-shear) and [null twist](../../../geodesic-congruence.md#null-twist) zero for these radial congruences.

There is a small parametrization distinction. The smooth field $X=-\partial_r$ is affine, since $\Gamma^a{}_{rr}=0$. The natural smooth field $Y=\partial_v+(f/2)\partial_r$ obeys $\nabla_Y Y=(f'/2)Y$. To meet part (a)'s affine convention, use an [affine rescaling of a null normal](../../../geodesic-congruence.md#affine-rescaling-of-a-null-normal) along the outgoing generators, with scaling equal to one on $S$. Its angular derivatives on $S$ then leave the projected derivative unchanged. The displayed [null expansions](../../../geodesic-congruence.md#null-expansion) are therefore precisely those for the affinely launched congruences, even though that convenient global expression for $Y$ is nonaffine away from its initial sphere.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

A future [trapped surface](../../../general-relativity.md#trapped-surface) is a closed spacelike two-surface for which both future orthogonal [null expansions](../../../geodesic-congruence.md#null-expansion) are strictly negative. Multiplying a future [null vector](../../../special-relativity.md#null-vector) normal by a positive function multiplies its [null expansion](../../../geodesic-congruence.md#null-expansion) by that function, so the signs are invariant under allowed normalization changes.

Here $\theta_X<0$ for every $r_0>0$. Thus the [Reissner-Nordstrom trapped spheres](../../../general-relativity.md#reissner-nordstrom-trapped-spheres) are exactly those with $f(r_0)<0$. Since $r_+>r_->0$,

$$
\boxed{S\text{ is future trapped precisely when }r_-<r_0<r_+.}
$$

At either horizon $\theta_Y=0$, so the spheres are marginal, rather than strictly [trapped surfaces](../../../general-relativity.md#trapped-surface). For $r_0>r_+$ or $0<r_0<r_-$, $\theta_Y>0$ and this future-trapping condition fails. In particular, being inside the outer [event horizon](../../../general-relativity.md#event-horizon) alone is insufficient to make every sphere trapped in the charged solution.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

One standard form of the [Penrose singularity theorem](../../../general-relativity.md#penrose-singularity-theorem) assumes a time-oriented [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime) with a noncompact [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface), the [null convergence condition](../../../general-relativity.md#null-convergence-condition) $R_{ab}k^ak^b\geq0$ for every [null vector](../../../special-relativity.md#null-vector) $k$, and a closed future [trapped surface](../../../general-relativity.md#trapped-surface). It concludes **future null geodesic incompleteness**: some future-inextendible [null geodesic](../../../special-relativity.md#null-geodesic) has a finite upper endpoint of its [affine parameter](../../../riemannian-geometry.md#affine-parameter).

The focusing mechanism is the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation). The normal generators have zero [null twist](../../../geodesic-congruence.md#null-twist), so

$$
\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}-R_{ab}k^ak^b\leq-\frac12\theta^2.
$$

An initial $\theta_0<0$ therefore gives a [conjugate point to a spacelike surface](../../../geodesic-congruence.md#conjugate-point-to-a-spacelike-surface) within affine distance at most $2/|\theta_0|$, assuming the generator can be continued that far. Such a generator ceases to lie on the [achronal boundary](../../../general-relativity.md#achronal-boundary) after its first focal point. Compactness of the [trapped surface](../../../general-relativity.md#trapped-surface) supplies a uniform bound for all normalized initial null normals. Future completeness would consequently make its future boundary compact. Projection along timelike curves to a connected [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) is injective on the [achronal boundary](../../../general-relativity.md#achronal-boundary) and has open image. Compactness makes the image closed as well; the nonempty image must therefore be the entire hypersurface, contradicting its noncompactness. This explains why the global assumptions supplement local focusing.

For [Reissner-Nordstrom spacetime](../../../general-relativity.md#reissner-nordstrom-spacetime), the Maxwell [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) satisfies the [null energy condition](../../../general-relativity.md#null-energy-condition); the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) imply the required [null convergence condition](../../../general-relativity.md#null-convergence-condition). The spheres in the band just found are closed and trapped. Apply the theorem to a [maximal Cauchy development](../../../general-relativity.md#maximal-cauchy-development) with a noncompact [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) and containing one such sphere. That [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime) must be future [null-geodesically incomplete](../../../general-relativity.md#null-geodesic-incompleteness).

The [Penrose theorem at a Cauchy horizon](../../../general-relativity.md#penrose-theorem-at-a-cauchy-horizon) needs care: the full maximal analytic [Reissner-Nordstrom spacetime](../../../general-relativity.md#reissner-nordstrom-spacetime) has inner [Cauchy horizons](../../../general-relativity.md#cauchy-horizon) and is not globally hyperbolic. It does not satisfy every hypothesis of the displayed theorem. In the exact solution some incomplete geodesics of the globally hyperbolic development reach a smoothly extendible [Cauchy horizon](../../../general-relativity.md#cauchy-horizon) in finite [affine parameter](../../../riemannian-geometry.md#affine-parameter). The theorem asserts incompleteness of the development, not that every such endpoint is a curvature singularity. The separate curvature singularity at $r=0$ does not justify silently dropping the theorem's global hypothesis.

## 3

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An isolated uncharged collapsing star initially has higher [multipole moments](../../../physics.md#multipole-moment) and possibly time-dependent motion. The changing exterior emits [gravitational waves](../../../general-relativity.md#gravitational-wave), carrying away energy and nonspherical structure. Perturbations of the final [black hole](../../../general-relativity.md#black-hole) decay, so the late exterior is expected to approach a [stationary spacetime](../../../general-relativity.md#stationary-spacetime).

Under the regularity, asymptotic flatness, and connected-horizon hypotheses of the [black-hole uniqueness theorem](../../../general-relativity.md#black-hole-uniqueness-theorem), a stationary four-dimensional vacuum [black hole](../../../general-relativity.md#black-hole) is a [Kerr black hole](../../../general-relativity.md#kerr-black-hole). Since the electric charge is zero, its intrinsic parameters are

$$
\boxed{M\quad\text{and}\quad J,\qquad a=J/M.}
$$

The [black-hole no-hair theorem](../../../general-relativity.md#black-hole-no-hair-theorem) expresses the loss of independently specifiable higher multipoles: those of the final [Kerr black hole](../../../general-relativity.md#kerr-black-hole) are determined by $M,J$. The direction of the rotation axis can be chosen by orienting the coordinates and is not an additional intrinsic parameter of the geometry.

This is a statement about the settled, isolated exterior in classical [general relativity](../../../general-relativity.md), conditional on settling and the hypotheses of the [black-hole uniqueness theorem](../../../general-relativity.md#black-hole-uniqueness-theorem). It does not describe the entire radiating collapse spacetime with only two numbers, nor does it extend unchanged to additional long-range matter fields.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Write $A=r^2+a^2$, $s=\sin\theta$, $\Sigma=A-a^2s^2$, and $\Delta=A-2Mr$. Use [ingoing Kerr coordinates](../../../general-relativity.md#ingoing-kerr-coordinates), so $dt=dv-A\,dr/\Delta$ and $d\phi=d\chi-a\,dr/\Delta$. To see the cancellations without expanding every term, write the [Kerr metric](../../../general-relativity.md#kerr-metric) in the equivalent form

$$
ds^2=-\frac\Delta\Sigma(dt-a s^2d\phi)^2+\frac\Sigma\Delta dr^2+\Sigma d\theta^2+\frac{s^2}\Sigma(A\,d\phi-a\,dt)^2.
$$

The combinations become

$$
dt-a s^2d\phi=dv-a s^2d\chi-\frac\Sigma\Delta dr,\qquad A\,d\phi-a\,dt=A\,d\chi-a\,dv.
$$

The first square contributes $-\Sigma dr^2/\Delta$, cancelling the explicit radial term. Expanding the remaining terms gives

$$
\boxed{\begin{aligned}
ds^2={}&-\left(1-\frac{2Mr}\Sigma\right)dv^2+2\,dv\,dr-\frac{4Mar s^2}\Sigma\,dv\,d\chi-2a s^2\,dr\,d\chi\\
&+\Sigma\,d\theta^2+\left(A+\frac{2Ma^2r s^2}\Sigma\right)s^2d\chi^2.
\end{aligned}}
$$

There is no denominator $\Delta$ in this [Lorentzian metric](../../../general-relativity.md#lorentzian-metric). At the outer horizon $r_+=M+\sqrt{M^2-a^2}$, $\Sigma>0$ and the components are smooth. The determinant is $-\Sigma^2\sin^2\theta$, so away from the usual polar-coordinate degeneracy the metric is nondegenerate and extends across $r_+$. The axis can be covered by regular angular charts. Thus the [Boyer-Lindquist coordinates](../../../general-relativity.md#boyer-lindquist-coordinates) are singular there, while the [ingoing Kerr coordinates](../../../general-relativity.md#ingoing-kerr-coordinates) are regular at the future horizon.

For physical nonextremality the invariant parameter condition is $M>|a|$, $M>0$. The printed $M>a$ is sufficient when the rotation orientation has been chosen so that $a\geq0$; without that convention it needs the absolute value.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The change to [ingoing Kerr coordinates](../../../general-relativity.md#ingoing-kerr-coordinates) adds functions of $r$ to $t$ and $\phi$, and leaves $r,\theta$ unchanged. Differentiating at fixed $r,\theta,\phi$ therefore gives $\partial_t v=1$ and $\partial_t\chi=0$. Differentiating at fixed $r,\theta,t$ gives $\partial_\phi\chi=1$ and $\partial_\phi v=0$. Hence the two [Killing vector fields](../../../general-relativity.md#killing-vector-field) are

$$
\boxed{k=\partial_v,\qquad m=\partial_\chi.}
$$

They remain the stationary and axial [Killing vector fields](../../../general-relativity.md#killing-vector-field); the coordinate change does not mix their generators with $\partial_r$.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

The inverse [Kerr metric](../../../general-relativity.md#kerr-metric) in [ingoing Kerr coordinates](../../../general-relativity.md#ingoing-kerr-coordinates) gives the raised normal to a surface of constant $r$:

$$
n^a=g^{ar}=\frac1\Sigma\left(A\,\partial_v+\Delta\,\partial_r+a\,\partial_\chi\right)^a,\qquad n^2=g^{rr}=\frac\Delta\Sigma.
$$

On $r=r_+$, $\Delta=0$, so the normal is null and tangent to the horizon. It reduces to

$$
n^a\big|_H=\frac{r_+^2+a^2}{\Sigma_H}\left(k^a+\frac a{r_+^2+a^2}m^a\right).
$$

A constant linear combination of the two [Killing vector fields](../../../general-relativity.md#killing-vector-field) is again a [Killing vector field](../../../general-relativity.md#killing-vector-field). Therefore $k+\Omega_Hm$ is normal to this [null hypersurface](../../../general-relativity.md#null-hypersurface), establishing that it is a [Killing horizon](../../../general-relativity.md#killing-horizon), with [Kerr horizon angular velocity](../../../general-relativity.md#kerr-horizon-angular-velocity)

$$
\boxed{\Omega_H=\frac a{r_+^2+a^2}=\frac a{2Mr_+}.}
$$

The second equality uses $\Delta(r_+)=0$. This normal calculation proves hypersurface orthogonality on the horizon, rather than merely proving that the proposed vector happens to have zero norm there.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

A generator of the [Killing horizon](../../../general-relativity.md#killing-horizon) is an orbit of $k+\Omega_Hm$. In [ingoing Kerr coordinates](../../../general-relativity.md#ingoing-kerr-coordinates) it has constant $r=r_+$ and $\theta$, with $d\chi/dv=\Omega_H$. Since the coordinate shifts depend only on $r$, this is also $d\phi/dt=\Omega_H$ in the limiting [Boyer-Lindquist coordinates](../../../general-relativity.md#boyer-lindquist-coordinates) description.

Thus **$\Omega_H$ is the angular velocity of the horizon relative to the nonrotating stationary frame at infinity**. The stationary [Killing vector field](../../../general-relativity.md#killing-vector-field) $k$ is normalized to unit time translation there, while the axial [Killing vector field](../../../general-relativity.md#killing-vector-field) has $2\pi$-periodic orbits. This normalization makes the [Kerr horizon angular velocity](../../../general-relativity.md#kerr-horizon-angular-velocity) physically definite. It describes the rotation of the null generators and the dragging of inertial frames, not a material solid surface rotating through space. In the [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime) limit $a=0$, $\Omega_H=0$.

<h4 id="3/b/v">v</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/v/solution">Solution</h5>

↑ **Parent:** [V](#3/b/v)

For the [scalar wave separation in Kerr spacetime](../../../general-relativity.md#scalar-wave-separation-in-kerr-spacetime), continue to use $A=r^2+a^2$ and $s=\sin\theta$. First verify the determinant in the hint. Direct multiplication of the covariant $t,\phi$ components gives

$$
\begin{aligned}
\Sigma^2(g_{tt}g_{\phi\phi}-g_{t\phi}^2)&=-s^2(\Delta-a^2s^2)(A^2-\Delta a^2s^2)-a^2s^4(A-\Delta)^2\\
&=-\Delta s^2(A-a^2s^2)^2=-\Delta s^2\Sigma^2.
\end{aligned}
$$

Hence the block determinant is $-\Delta\sin^2\theta$. Inverting this block gives

$$
g^{tt}=-\frac{A^2-\Delta a^2s^2}{\Sigma\Delta},\qquad g^{t\phi}=-\frac{a(A-\Delta)}{\Sigma\Delta},\qquad g^{\phi\phi}=\frac{\Delta-a^2s^2}{\Sigma\Delta s^2}.
$$

The other inverse components are $g^{rr}=\Delta/\Sigma$, $g^{\theta\theta}=1/\Sigma$, and $\sqrt{-g}=\Sigma s$. The [covariant wave operator](../../../quantum-field-theory.md#covariant-wave-operator) on a scalar consequently has the divergence form

$$
\Box\Psi=\frac1{\Sigma s}\partial_\mu(\Sigma s\,g^{\mu\nu}\partial_\nu\Psi).
$$

Let $m_\phi$ denote the azimuthal mode number, to distinguish it from the axial vector $m$. Insert the mode $\Psi=e^{-i\omega t+i m_\phi\phi}R(r)\Theta(\theta)$ in the massless [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation). Single-valuedness makes $m_\phi$ an integer. The $t,\phi$ derivatives give

$$
\Sigma\left(-\omega^2g^{tt}+2\omega m_\phi g^{t\phi}-m_\phi^2g^{\phi\phi}\right)=\frac{(A\omega-a m_\phi)^2}{\Delta}+2a\omega m_\phi-a^2\omega^2\sin^2\theta-\frac{m_\phi^2}{\sin^2\theta}.
$$

With $K(r)=A\omega-a m_\phi$, division by the mode factor gives, on patches where $R\Theta\ne0$,

$$
\frac{(\Delta R')'}R+\frac{K^2}\Delta+2a\omega m_\phi-a^2\omega^2+\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}+a^2\omega^2\cos^2\theta-\frac{m_\phi^2}{\sin^2\theta}=0.
$$

The radial and angular expressions must be opposite constants. Defining the [separation constant](../../../partial-differential-equation.md#separation-constant) as $\Lambda$, we obtain the two [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation)

$$
\boxed{\frac1{\sin\theta}\frac d{d\theta}\left(\sin\theta\frac{d\Theta}{d\theta}\right)+\left(a^2\omega^2\cos^2\theta-\frac{m_\phi^2}{\sin^2\theta}+\Lambda\right)\Theta=0,}
$$



$$
\boxed{\frac d{dr}\left(\Delta\frac{dR}{dr}\right)+\left[\frac{((r^2+a^2)\omega-a m_\phi)^2}{\Delta}-a^2\omega^2+2a\omega m_\phi-\Lambda\right]R=0.}
$$

These equations also hold at zeros of a mode by continuity, without dividing there. Regular angular solutions are [scalar spheroidal harmonics](../../../general-relativity.md#scalar-spheroidal-harmonic), with discrete $\Lambda=\Lambda_{\ell m_\phi}(a\omega)$. For $a\omega=0$ the angular equation becomes the [associated Legendre function](../../../differential-equation.md#associated-legendre-function) equation, with $\Lambda=\ell(\ell+1)$ and $\ell\geq|m_\phi|$, providing a useful check of the signs and normalization. The radial function here is exactly $R$ in the chosen ansatz, without an additional factor of $1/r$.

## 4

↑ **Parent:** [Paper 52](paper-52.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Fix a classical [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime) with [metric signature](../../../topology.md#metric-signature) $(-+++)$; in this solution take $\hbar=1$. A free real [Klein-Gordon field](../../../quantum-field-theory.md#klein-gordon-field) can be specified by

$$
S[\phi]=-\frac12\int\sqrt{-g}\,d^4x\left(g^{ab}\nabla_a\phi\nabla_b\phi+(\mu^2+\xi\mathcal R)\phi^2\right),\qquad (\Box-\mu^2-\xi\mathcal R)\phi=0,
$$

where $\mu$ is its mass, $\xi$ its curvature coupling and $\mathcal R$ the [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). [Global hyperbolicity](../../../general-relativity.md#globally-hyperbolic-spacetime) ensures a well-posed initial-value problem on a [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) $\Sigma$ and the existence of retarded and advanced propagators. Thus compactly supported field and normal-derivative data determine a classical solution. This fixes the dynamics, but not a [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum).

For real solutions with suitable support or falloff, the [symplectic form on scalar-field solutions](../../../quantum-field-theory.md#symplectic-form-on-scalar-field-solutions) is

$$
\Omega(\phi_1,\phi_2)=\int_\Sigma d\Sigma\,\left(\phi_1n^a\nabla_a\phi_2-\phi_2n^a\nabla_a\phi_1\right),
$$

with $n$ the future unit normal. The field equation makes the current conserved, so this [symplectic form](../../../symplectic-geometry.md#symplectic-form) is independent of $\Sigma$ when boundary flux vanishes. Quantize the initial data by the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation): with $\pi=n^a\nabla_a\phi$ and the delta function defined relative to $d\Sigma$, $[\widehat\phi(x),\widehat\pi(y)]=i\delta_\Sigma(x,y)$ and the two equal-field commutators vanish. Equivalently, construct the field algebra using the causal propagator. A state on that algebra is additional input.

To construct a particle representation, complexify the classical solution space. Its conserved [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product) is

$$
(u,v)_{KG}=i\int_\Sigma d\Sigma\,\left(u^*n^a\nabla_av-vn^a\nabla_au^*\right).
$$

It is indefinite on all complex solutions. Choose a complete positive-norm subspace and an orthonormal mode basis $u_i$ with $(u_i,u_j)=\delta_{ij}$, $(u_i^*,u_j^*)=-\delta_{ij}$ and $(u_i,u_j^*)=0$. Such a choice is encoded by a compatible [complex structure on the Klein-Gordon solution space](../../../quantum-field-theory.md#complex-structure-on-the-klein-gordon-solution-space). Its positive subspace gives the one-particle [Hilbert space](../../../hilbert-space.md), and the associated [bosonic Fock space](../../../quantum-field-theory.md#bosonic-fock-space) contains symmetrized many-particle states. The field expansion is

$$
\widehat\phi=\sum_i(a_i u_i+a_i^\dagger u_i^*),\qquad [a_i,a_j^\dagger]=\delta_{ij},\qquad a_i|0\rangle=0.
$$

The [creation operator](../../../quantum-mechanics.md#creation-operator) $a_i^\dagger$ adds a particle in mode $i$, the [annihilation operator](../../../quantum-mechanics.md#annihilation-operator) removes one, and the [number operator](../../../quantum-mechanics.md#number-operator) is $N_i=a_i^\dagger a_i$. For continuous mode labels the sums and Kronecker deltas become integrals and delta functions, or one can work with normalized wave packets.

The ambiguity is precisely that the field equation and [global hyperbolicity](../../../general-relativity.md#globally-hyperbolic-spacetime) do not select that positive subspace. A different normalized basis may mix $u_j$ and $u_j^*$ by a [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation), and then its [annihilation operators](../../../quantum-mechanics.md#annihilation-operator) mix $a_j$ and $a_j^\dagger$. Its [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) and [number operators](../../../quantum-mechanics.md#number-operator) differ. The [Hadamard condition](../../../quantum-field-theory.md#hadamard-condition) constrains physically acceptable short-distance singularities and allows local renormalization, but it still leaves many states. Hence there is generally no observer-independent particle count on an arbitrary dynamical geometry.

In a stable [strictly stationary spacetime](../../../general-relativity.md#strictly-stationary-spacetime), a globally future timelike [Killing vector field](../../../general-relativity.md#killing-vector-field) $K$ gives a preferred time translation. Fix its normalization and suitable boundary conditions, and choose [positive-frequency solutions](../../../quantum-field-theory.md#positive-frequency-solution) satisfying $i\mathcal L_Ku=\omega u$ with $\omega>0$. The corresponding positive spectral subspace gives the preferred [vacuum state in a stationary spacetime](../../../quantum-field-theory.md#vacuum-state-in-a-stationary-spacetime). Unitary changes of basis within it leave the vacuum and the particle notion unchanged. This construction assumes a well-defined positive stationary generator; stationarity by itself is insufficient if $K$ becomes spacelike, as in a [Kerr ergoregion](../../../general-relativity.md#kerr-ergoregion), or if unstable or zero modes obstruct the ground-state construction. It selects a preferred ground state under the stated assumptions, not a unique state among all thermal and excited states.

If the geometry is suitably stationary in the asymptotic past and future, choose those preferred mode spaces separately, giving the [in-vacuum](../../../quantum-field-theory.md#in-vacuum) and [out-vacuum](../../../quantum-field-theory.md#out-vacuum). Propagate the past modes through the intervening region using the field equation and compare them to the future modes using the conserved [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product). Adopt the convention

$$
u_i^{\rm out}=\sum_j\left(\alpha_{ij}u_j^{\rm in}+\beta_{ij}u_j^{{\rm in}*}\right),\qquad \alpha_{ij}=(u_j^{\rm in},u_i^{\rm out})_{KG},\quad \beta_{ij}=-(u_j^{{\rm in}*},u_i^{\rm out})_{KG}.
$$

The [canonical identities for a bosonic Bogoliubov transformation](../../../quantum-field-theory.md#canonical-identities-for-a-bosonic-bogoliubov-transformation) read $\alpha\alpha^\dagger-\beta\beta^\dagger=I$ and $\alpha\beta^T=\beta\alpha^T$. Extracting the future [annihilation operator](../../../quantum-mechanics.md#annihilation-operator) with the same inner product gives

$$
b_i=(u_i^{\rm out},\widehat\phi)_{KG}=\sum_j\left(\alpha_{ij}^*a_j-\beta_{ij}^*a_j^\dagger\right).
$$

In the [in-vacuum](../../../quantum-field-theory.md#in-vacuum), only $\langle a_j a_k^\dagger\rangle=\delta_{jk}$ contributes to $\langle b_i^\dagger b_i\rangle$. Therefore the [particle number from Bogoliubov coefficients](../../../quantum-field-theory.md#particle-number-from-bogoliubov-coefficients) is

$$
\boxed{\langle0_{\rm in}|N_i^{\rm out}|0_{\rm in}\rangle=\sum_j|\beta_{ij}|^2.}
$$

Nonzero $\beta$ is the production of future particles from the past vacuum. Summing over future modes gives the total expected particle number when that sum is finite. For infinitely many modes, a [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator) $\beta$ is the condition for unitary implementability between these pure [bosonic Fock space](../../../quantum-field-theory.md#bosonic-fock-space) representations; finite-volume or wave-packet calculations must respect the relevant measures and convergence. **Particle production is determined by the negative-frequency mixing**, rather than by identifying a single instantaneous vacuum throughout the time-dependent region.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [laws of black-hole mechanics](../../../general-relativity.md#laws-of-black-hole-mechanics) initially relate geometric quantities in a way resembling [thermodynamics](../../../thermodynamics.md). [Hawking radiation](../../../general-relativity.md#hawking-radiation) supplies a physical temperature: in units $c=1$, while displaying $G,\hbar,k_B$,

$$
\boxed{T_H=\frac{\hbar\kappa}{2\pi k_B},\qquad S_{\rm BH}=\frac{k_B A}{4G\hbar}.}
$$

The [Hawking temperature](../../../general-relativity.md#hawking-temperature) $T_H$ is measured with the stationary time normalized at infinity. The radiation's thermal occupation factor is physically observable; propagation to infinity also introduces [greybody factors](../../../general-relativity.md#greybody-factor), so the distant spectrum need not be a perfect blackbody spectrum at every frequency.

The [Zeroth law of black-hole mechanics](../../../general-relativity.md#zeroth-law-of-black-hole-mechanics) says that [surface gravity](../../../general-relativity.md#surface-gravity) $\kappa$ is constant on a stationary [Killing horizon](../../../general-relativity.md#killing-horizon) under its standard hypotheses. Through the [Hawking temperature](../../../general-relativity.md#hawking-temperature), this becomes uniform equilibrium temperature. The [First law of black-hole mechanics](../../../general-relativity.md#first-law-of-black-hole-mechanics) is

$$
\delta M=\frac\kappa{8\pi G}\delta A+\Omega_H\delta J+\Phi_H\delta Q.
$$

Using $T_H$ identifies its area term as $T_H\delta S_{\rm BH}$. Integrating $\delta S_{\rm BH}=k_B\delta A/(4G\hbar)$ gives the [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy), up to an additive constant. Thus $M$ is the energy, the angular and charge terms are work terms, and the geometrical law is the ordinary thermodynamic first law with a fixed entropy normalization.

The [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics), or [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem), gives nondecreasing area in the classical setting with the requisite energy and predictability assumptions. It corresponds to increasing [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy). Semiclassical [black-hole evaporation](../../../general-relativity.md#black-hole-evaporation) can decrease the area: the classical [null energy condition](../../../general-relativity.md#null-energy-condition) need not hold for the quantum expectation of the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor). The appropriate extension is the [generalized second law](../../../general-relativity.md#generalized-second-law), that $S_{\rm BH}+S_{\rm outside}$ does not decrease, with the exterior entropy and its renormalization treated consistently. Hawking's temperature identification motivates this law; thermality alone does not prove every form of it.

The [third law of black-hole mechanics](../../../general-relativity.md#third-law-of-black-hole-mechanics) is the unattainability, by an admissible finite physical process, of zero [surface gravity](../../../general-relativity.md#surface-gravity). With [Hawking temperature](../../../general-relativity.md#hawking-temperature) it becomes unattainability of absolute zero. It is not the assertion that an [extremal black hole](../../../general-relativity.md#extremal-black-hole) has vanishing entropy: its area can remain nonzero when $\kappa=0$.

For a [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime), $\kappa=1/(4GM)$ and $A=16\pi G^2M^2$, giving $T_H=\hbar/(8\pi k_BGM)$ and $S_{\rm BH}=4\pi k_BGM^2/\hbar$. Their product satisfies $T_H\,dS_{\rm BH}=dM$, explicitly checking the first law. **Quantum radiation turns the temperature and entropy in the mechanical analogy into physical thermodynamic quantities.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
