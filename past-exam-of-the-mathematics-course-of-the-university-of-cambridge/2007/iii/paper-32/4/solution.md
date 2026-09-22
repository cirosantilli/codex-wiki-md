<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work on a finite interval $[0,T]$ with a fixed initial point $y_0\in\mathbb R^m$. To give a clean global statement, assume $V_0,V_1,\ldots,V_d$ are bounded vector fields with bounded continuous derivatives through order three. Consider the [Stratonovich integral](../../../../../stratonovich-integral.md) form of the [stochastic differential equation](../../../../../stochastic-differential-equation.md)

$$
dY_t=V_0(Y_t)\,dt+\sum_{i=1}^d V_i(Y_t)\circ dB^i_t,\qquad Y_0=y_0.
$$

For a control in the [Cameron-Martin space of Wiener measure](../../../../../cameron-martin-space-of-wiener-measure.md),

$$
H=\{h:h(0)=0,\ h\text{ absolutely continuous},\ \dot h\in L^2([0,T];\mathbb R^d)\},
$$

let $y^h$ solve the controlled [ordinary differential equation](../../../../../ordinary-differential-equation.md)

$$
\dot y^h_t=V_0(y^h_t)+\sum_{i=1}^d V_i(y^h_t)\dot h^i_t,\qquad y^h_0=y_0.
$$

The [Stroock-Varadhan support theorem](../../../../../stroock-varadhan-support-theorem.md) says, in the [uniform metric](../../../../../uniform-metric.md) on continuous paths,

$$
\boxed{\operatorname{supp}\mathcal L(Y)
=\overline{\{y^h:h\in H\}}^{\|\cdot\|_\infty}.}
$$

Thus a path is in the [support of a measure](../../../../../support-of-a-measure.md) of the diffusion precisely when it can be approximated by these deterministic controlled trajectories. There is no ellipticity assumption: the allowed controls and vector fields already encode any restrictions on reachability.

The central point of the rough-path proof is that ordinary uniform approximation of the driver does not make the solution map continuous. Small planar loops can have small amplitude but accumulated area of fixed size, and vector fields with a nonzero [Lie bracket](../../../../../lie-bracket.md) detect that area. The correct driver is [enhanced Brownian motion](../../../../../enhanced-brownian-motion.md) $\mathbf B$, including [Lévy area](../../../../../levy-area.md). Fix $2<p<3$. The [universal limit theorem](../../../../../universal-limit-theorem.md) gives a continuous map

$$
\Phi:\mathbf X\longmapsto Y^{\mathbf X}
$$

from the geometric $p$-variation rough-path space to solution paths. It agrees with the controlled [ordinary differential equation](../../../../../ordinary-differential-equation.md) when $\mathbf X=S_2(h)$. Adding the time coordinate, with its mixed integrals defined by integration against $dt$ and [integration by parts](../../../../../integration-by-parts.md), incorporates $V_0$ without changing the continuity argument. This is the role of the [universal limit theorem](../../../../../universal-limit-theorem.md): it turns a support problem for all these nonlinear diffusions into a support problem for one enhanced driving process.

For $\mathbf X=\mathbf B$, the [rough differential equation](../../../../../rough-differential-equation.md) is the stated Stratonovich equation. Its second-order increment includes

$$
\sum_iV_i(Y_s)B^i_{s,t}
+\sum_{i,j}DV_j(Y_s)V_i(Y_s)\mathbb B^{ij}_{s,t}.
$$

Replacing the [Stratonovich integral](../../../../../stratonovich-integral.md) in the second level by its [Itô integral](../../../../../ito-integral.md) expression contributes $\tfrac12\sum_iDV_iV_i\,dt$, which is exactly the Stratonovich-to-Itô correction. Polygonal convergence from Question 3 and the [universal limit theorem](../../../../../universal-limit-theorem.md) therefore give the Wong-Zakai approximation: the ordinary equations driven by $B^n$ converge to this Stratonovich diffusion.

It remains to establish the [support of enhanced Brownian motion](../../../../../support-of-enhanced-brownian-motion.md):

$$
\operatorname{supp}\mathcal L(\mathbf B)
=K:=\overline{\{S_2(h):h\in H\}}^{d_p}.
$$

One inclusion follows immediately from Question 3. Every polygonal $B^n$ belongs to $H$, and $S_2(B^n)\to\mathbf B$ almost surely in the [rough path metric](../../../../../rough-path-metric.md). Since $K$ is closed, $\mathbf B\in K$ almost surely, whence its support is contained in $K$. This alone does not prove the reverse inclusion: convergence of random approximations does not automatically give positive mass near every control.

For that inclusion, take dyadic mesh $\delta_n=T2^{-n}$ and write

$$
B=B^n+R^n.
$$

On each grid interval $R^n$ is a pinned [Brownian bridge](../../../../../brownian-bridge.md). The bridges are mutually independent and independent of the grid values defining $B^n$, by the Gaussian projection formula. Their canonical Stratonovich enhancement $\mathbf R^n$ is therefore independent of $B^n$. It is important to enhance the bridge residual itself, including its area, rather than infer area smallness from its uniform size.

The bridge enhancement tends to the zero rough path in probability. Here are the estimates behind this assertion. A bridge on an interval of length $\delta_n$ scales as $\sqrt{\delta_n}$ times a unit bridge; its full antisymmetric area has mean zero, moments of order $\delta_n$, and second moment of order $\delta_n^2$. Since its endpoint displacement is zero, at grid points the cumulative second level is just the sum of the independent bridge areas. The [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) gives

$$
\mathbb E\max_{k\le2^n}\left|\sum_{j<k}A^n_j\right|^2
\le4\sum_{j<2^n}\mathbb E|A^n_j|^2
\le C T\delta_n\longrightarrow0.
$$

Partial intervals at the two ends contribute bridge increments and at most two local areas. Bridge scaling, Gaussian moment bounds and the corresponding iterated-integral estimates yield, uniformly in $n$ and for arbitrarily large $q$,

$$
\mathbb E|R^n_{s,t}|^q\le C_q|t-s|^{q/2},\qquad
\mathbb E|\mathbb R^n_{s,t}|^q\le C_q|t-s|^q.
$$

For an interval crossing several grid cells, the full-cell second levels are independent centered areas, whose sum has moments bounded by $C_q((t-s)\delta_n)^{q/2}$; the two boundary pieces and their cross product satisfy the displayed bound as well. For an interval inside one cell these are the usual scaled bridge increment and area bounds. At each fixed pair $(s,t)$ both levels converge to zero in probability: the first-level variance is $O(\delta_n)$, and the second-level second moment is $O((t-s)\delta_n+\delta_n^2)$ for sufficiently fine grids. The [Kolmogorov continuity theorem](../../../../../kolmogorov-continuity-theorem.md) gives uniformly bounded moments of a Hölder rough-path norm at any exponent $\beta<1/2$. Tightness, convergence on a dense set of pairs and interpolation to $\alpha<\beta$ now give $\rho_\alpha(\mathbf R^n,e)\to0$ in probability. Taking $1/p<\alpha<1/2$ gives $d_p(\mathbf R^n,e)\to0$ in probability.

Fix $h\in H$. Its polygonal interpolations $h^n$ converge to $h$ in the total-variation norm: their derivatives are the cell averages of $\dot h$, which converge in $L^2$, hence in $L^1$. Moreover $|h^n|_{1\text{-var}}\le|h|_{1\text{-var}}$. Thus $S_2(h^n)\to S_2(h)$ in the [rough path metric](../../../../../rough-path-metric.md).

The [rough path translation](../../../../../rough-path-translation.md) operation satisfies

$$
\mathbf B=T_{B^n}\mathbf R^n.
$$

For a [bounded variation](../../../../../total-variation-of-a-function.md) path $b$, translation adds $b$ at level one and, at level two, the mixed terms

$$
\int_s^t R_{s,r}\otimes db_r+
\int_s^t b_{s,r}\otimes dR_r+
\int_s^t b_{s,r}\otimes db_r.
$$

The second mixed term is defined by [integration by parts](../../../../../integration-by-parts.md). Their variation bounds show that translation is continuous, uniformly when $|b|_{1\text{-var}}$ is bounded, near the zero rough path. More explicitly the mixed second-level norms are bounded by a constant times $\|R\|_{p\text{-var}}|b|_{1\text{-var}}$; the other new second-level term is the [path signature](../../../../../signature-of-a-bounded-variation-path.md) of $b$.

Given a ball of radius $\varepsilon$ around $S_2(h)$, choose a sufficiently large $n$ so that $S_2(h^n)$ is close and

$$
\mathbb P(d_p(\mathbf R^n,e)<\eta)>0
$$

for the small $\eta$ supplied by translation continuity. The relevant variation bounds can be chosen uniformly in $n$, since the variations of the $h^n$ are uniformly bounded. For this fixed $n$, the event $|B^n-h^n|_{1\text{-var}}<\eta$ has positive probability: the finite vector of Brownian increments has an everywhere positive [Gaussian density](../../../../../multivariate-normal-density.md), and sufficiently small deviations of its vertices imply this variation bound. These two events are independent. On their intersection, translation continuity gives $d_p(\mathbf B,S_2(h))<\varepsilon$. Every ball around $S_2(h)$ therefore has positive probability. This proves $S_2(h)$ lies in the support, and taking closures gives $K$.

Finally, a continuous map between the separable path spaces in use satisfies

$$
\operatorname{supp}(\Phi_*\mu)=\overline{\Phi(\operatorname{supp}\mu)}.
$$

For one direction the measure is concentrated on its support. For the other, an open neighborhood of $\Phi(x)$ pulls back to an open neighborhood of a support point $x$, which has positive measure. Using continuity of $\Phi$ and the identity $\Phi(S_2(h))=y^h$ proves the boxed [Stroock-Varadhan support theorem](../../../../../stroock-varadhan-support-theorem.md). This separates the two ingredients: the probabilistic support calculation for [Brownian motion](../../../../../brownian-motion-split.md) and area, and the deterministic continuity supplied by the [universal limit theorem](../../../../../universal-limit-theorem.md).

If the diffusion is instead presented as an [Itô integral](../../../../../ito-integral.md) equation with drift $b$, the controlled equation must use

$$
\boxed{V_0=b-\tfrac12\sum_iDV_iV_i.}
$$

Using $b$ unchanged in the controlled equation would generally give the wrong support description. The result above states explicit sufficient smoothness and nonexplosion assumptions; extensions to more general coefficients require the usual localization, not an unqualified assertion for arbitrary vector fields.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
