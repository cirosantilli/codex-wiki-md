# Paper 64

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_64.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_64.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $\operatorname{TV}(u)=|Du|(\Omega)$ for the [total variation seminorm on a domain](../../../inverse-problem.md#total-variation-seminorm-on-a-domain). For a [locally integrable](../../../distribution-theory.md#locally-integrable-function) real function its dual definition is

$$
|Du|(\Omega)=\sup\left\{\int_\Omega u\,\operatorname{div}\varphi\,dx:\varphi\in C_c^1(\Omega;\mathbb R^2),\ |\varphi(x)|\le1\right\}.
$$

The [bounded-variation space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) consists of functions $u\in L^1(\Omega)$ with finite $|Du|(\Omega)$, equipped with $\|u\|_{BV}=\|u\|_1+|Du|(\Omega)$. In the equivalent [distributional derivative](../../../distribution-theory.md#distributional-derivative) description, $Du$ is a finite vector-valued [Radon measure](../../../measure-theory.md#radon-measure) and $|Du|$ is its [total variation measure](../../../measure-theory.md#variation-measure).

To establish [completeness of the bounded-variation space](../../../inverse-problem.md#completeness-of-the-bounded-variation-space), let $(u_n)$ be [Cauchy](../../../real-analysis.md#cauchy-sequence) in this [norm](../../../functional-analysis.md#norm). Completeness of $L^1$ gives $u_n\to u$ in $L^1$. Given $\varepsilon>0$, choose $N$ so that $\|u_n-u_m\|_{BV}<\varepsilon$ whenever $m,n\ge N$. For fixed $n\ge N$, the given [lower semicontinuity](../../../calculus.md#lower-semicontinuity) yields

$$
|D(u_n-u)|(\Omega)\le\liminf_{m\to\infty}|D(u_n-u_m)|(\Omega).
$$

Since $\|u_n-u_m\|_1\to\|u_n-u\|_1$, we obtain $\|u_n-u\|_1+|D(u_n-u)|(\Omega)\le\varepsilon$. In particular $u_n-u$ has finite variation; the [triangle inequality](../../../topological-analysis.md#triangle-inequality) then puts $u$ in the [BV space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain). The same bound proves convergence in the full [norm](../../../functional-analysis.md#norm), so this is a [Banach space](../../../banach-space.md).

For the disk data, put $B=B(0,R)$ and assume $\alpha>0$. The exact [total variation denoising of a disk](../../../inverse-problem.md#total-variation-denoising-of-a-disk) is

$$
\boxed{u_*=(1-2\alpha/R)_+\chi_B.}
$$

Here $(s)_+=\max(s,0)$ is the [positive part](../../../function.md#positive-part-of-a-real-valued-function). A [total variation calibration](../../../inverse-problem.md#total-variation-calibration) certifies global optimality, including competitors that are not radial or piecewise constant. Define the bounded [vector field](../../../calculus.md#vector-field)

$$
z(x)=\begin{cases}x/R,&|x|\le R,\\Rx/|x|^2,&|x|>R.\end{cases}
$$

It has $|z|\le1$. Its normal component is [continuous](../../../calculus.md#continuous-function) across the circle, so the [distributional divergence](../../../calculus.md#distributional-divergence) has no extra boundary measure. Direct differentiation gives $q=\operatorname{div}z=(2/R)\chi_B$. The dual definition implies $\int vq\le\operatorname{TV}(v)$: for the standard $BV\cap L^2$ domain one can cut $z$ off at radius $L$, with the error bounded by $C L^{-1}\int_{L<|x|<2L}|v|\to0$, and then smooth the test field. In the larger [homogeneous bounded-variation space](../../../inverse-problem.md#homogeneous-bounded-variation-space), the same error is bounded by $C\|v\|_{L^2(L<|x|<2L)}\to0$. Thus both usual whole-plane formulations give the same certificate.

Use the [perimeter](../../../inverse-problem.md#perimeter) identity $\operatorname{TV}(\chi_B)=2\pi R$ and $|B|=\pi R^2$. If $c=1-2\alpha/R>0$, then $\int c\chi_Bq=2\pi Rc=\operatorname{TV}(c\chi_B)$ and $u_*-g+\alpha q=0$. Consequently every competitor $v$ satisfies

$$
\begin{aligned}
E(v)-E(u_*)&\ge\alpha\langle q,v-u_*\rangle+\langle u_*-g,v-u_*\rangle+\tfrac12\|v-u_*\|_2^2\\
&=\tfrac12\|v-u_*\|_2^2\ge0.
\end{aligned}
$$

If $\alpha\ge R/2$, replace $z$ by $z_\alpha=(R/(2\alpha))z$. Its [norm](../../../functional-analysis.md#norm) is still at most one, its divergence is $q_\alpha=\chi_B/\alpha$, and equality in the calibration holds at $u_*=0$. The identical comparison proves optimality and uniqueness of zero, including the threshold $\alpha=R/2$. The only general results used are completeness of $L^1$, [lower semicontinuity](../../../calculus.md#lower-semicontinuity) of variation, the indicator-perimeter identity, the distributional integration-by-parts/dual variation formula and the quadratic [norm](../../../functional-analysis.md#norm) identity. For $\alpha=0$, the unique squared-error [minimizer](../../../analysis.md#global-minimizer) is simply $g$.

## 2

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Positivity means $u>0$ almost everywhere, since the real [logarithm](../../../calculus.md#logarithm) must belong to $L^1$. A [positivity-preserving operator](../../../topological-vector-space.md#positivity-preserving-linear-operator-on-l1) gives $s=Tu\ge0$. For fixed $x$, the scalar [shifted Poisson data fidelity](../../../inverse-problem.md#shifted-poisson-data-fidelity) is $f_x(s)=s-g(x)\log(1+s)$, with

$$
f_x'(s)=1-\frac{g(x)}{1+s},\qquad f_x''(s)=\frac{g(x)}{(1+s)^2}>0.
$$

Composition with the [linear operator](../../../vector-space.md#linear-operator) $T$ proves [convexity](../../../real-analysis.md#convex-function) in $u$, and strict [convexity](../../../real-analysis.md#convex-function) holds along pairs whose forward images differ on a set of positive measure. The admissible class itself is [convex](../../../real-analysis.md#convex-function): the [concavity of the logarithm](../../../calculus.md#concavity-of-the-logarithm) gives $\log(\theta u+(1-\theta)v)\ge\theta\log u+(1-\theta)\log v$, controlling its negative part, while $\log^+w\le w$ controls its positive part.

Because $|\Omega|=1$ and $\log(1+s)\ge0$, the [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives the requested bound:

$$
\begin{aligned}
\int_\Omega[s-g\log(1+s)]\,dx
&\ge\|s\|_1-\|g\|_\infty\int_\Omega\log(1+s)\,dx\\
&\ge\|s\|_1-\|g\|_\infty\log(1+\|s\|_1)\\
&=\|Tu\|_1-\|g\|_\infty\log\|Tu+1\|_1.
\end{aligned}
$$

The final equality uses nonnegativity and the unit area. Since $t-G\log(1+t)\to\infty$, this controls the forward-image [norm](../../../functional-analysis.md#norm) on energy sublevels.

**The printed strictly positive problem has no [minimizer](../../../analysis.md#global-minimizer).** This is [nonattainment under strict positivity for shifted Poisson fidelity](../../../inverse-problem.md#nonattainment-under-strict-positivity-for-shifted-poisson-fidelity), rather than a failure of the coercivity calculation. Indeed, with $0<g<1$ and $s>0$, $\log(1+s)<s$ implies $f_x(s)>0$. Also $Tu$ cannot vanish identically for a strictly positive $u$. To see this, let $E_n=\{u\ge1/n\}$. If $Tu=0$, positivity and $0\le\chi_{E_n}\le nu$ give $T\chi_{E_n}=0$. But $\chi_{E_n}\to\chi_\Omega$ in $L^1$ and [continuity](../../../calculus.md#continuous-function) of $T$ would imply $T\chi_\Omega=0$, contradicting the hypothesis. Thus every admissible $u$ has positive fidelity and hence positive total energy.

Conversely, the constants $u_\varepsilon=\varepsilon\chi_\Omega$ are admissible, have zero [total variation](../../../real-analysis.md#total-variation), and satisfy

$$
0<E(u_\varepsilon)\le\varepsilon\|T\chi_\Omega\|_1\longrightarrow0.
$$

Their logarithms are integrable for each $\varepsilon>0$, but the [limit](../../../calculus.md#limit-of-a-function) is excluded. Therefore

$$
\boxed{\inf E=0,\qquad\operatorname{argmin}E=\varnothing\quad\text{in the printed domain}.}
$$

A bounded minimizing sequence and [bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness) do not repair a nonclosed positivity/[logarithm](../../../calculus.md#logarithm) constraint. In particular, a literal existence or uniqueness proof for that domain is impossible.

The natural correction is to minimize over $BV(\Omega)$ with $u\ge0$, omitting the unnecessary $\log u\in L^1$ condition: the fidelity only contains $\log(1+Tu)$, which is already integrable. Here is the full [existence for nonnegative shifted Poisson regularization](../../../inverse-problem.md#existence-for-nonnegative-shifted-poisson-regularization) argument, also valid for any bounded nonnegative data $g$. Let $G=\|g\|_\infty$, $m_G=\inf_{t\ge0}\{t-G\log(1+t)\}>-\infty$, and take a minimizing sequence of energy at most $C$. The displayed bound gives $\|Tu_n\|_1\le C_1$ and $\alpha\operatorname{TV}(u_n)\le C-m_G$. Write $c_n=\int_\Omega u_n\ge0$. The [Poincaré inequality for total variation](../../../inverse-problem.md#poincare-inequality-for-total-variation) and [mean control for positive imaging operators](../../../topological-vector-space.md#mean-control-for-positive-imaging-operators) yield

$$
c_n\|T\chi_\Omega\|_1\le\|Tu_n\|_1+\|T\|\|u_n-c_n\|_1
\le C_1+C_P\|T\|\operatorname{TV}(u_n).
$$

The denominator is nonzero, so the full $BV$ [norm](../../../functional-analysis.md#norm) is bounded. [Bounded-variation compactness](../../../inverse-problem.md#bounded-variation-compactness) gives $u_n\to u$ in $L^1$ along a subsequence, with $u\ge0$. [Continuity](../../../calculus.md#continuous-function) gives $Tu_n\to Tu$ in $L^1$. On $s\ge0$, $|f_x'(s)|\le1+G$, so the fidelity converges in the integral; [lower semicontinuity](../../../calculus.md#lower-semicontinuity) of variation completes the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations).

For the actual printed data $0<g<1$, the corrected problem has the **unique [minimizer](../../../analysis.md#global-minimizer) $u=0$**, even if $T$ is not [injective](../../../algebra.md#injective-function). Zero attains energy zero. Any other zero-energy candidate would have both $Tu=0$ and $\operatorname{TV}(u)=0$; on the connected square, zero variation makes $u$ a nonnegative constant, and $T\chi_\Omega\ne0$ forces that constant to vanish. For general positive bounded data, an [injective](../../../algebra.md#injective-function) $T$ is a sufficient uniqueness condition, because its fidelity is [strictly convex](../../../real-analysis.md#strictly-convex-function); injectivity is not a necessary condition in every instance.

In the finite-dimensional interpretation, let $\lambda_{ij}=1+(Tu)_{ij}$. Independent [Poisson observations](../../../discrete-probability-distribution.md#poisson-observation) with these intensities have negative [log-likelihood](../../../statistical-modelling.md#log-likelihood) $\sum_{ij}[\lambda_{ij}-g_{ij}\log\lambda_{ij}]+C(g)$. Removing the constant $\sum1$ gives precisely the stated fidelity. Thus the model is **Poisson counting noise with a unit background intensity**, or an approximate version of it for rescaled/[continuous](../../../calculus.md#continuous-function) grey values. Literal Poisson counts are integers; the constraint $0<g<1$ is a grey-value normalization, not a literal unscaled count sample.

## 3

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The bounded classical solution is the [heat-kernel convolution](../../../diffusion-equation.md#heat-kernel-convolution)

$$
\boxed{u(x,t)=\frac1{4\pi t}\int_{\mathbb R^2}\exp\!\left(-\frac{|x-y|^2}{4t}\right)g(y)\,dy,\qquad t>0.}
$$

The two-dimensional [heat kernel](../../../diffusion-equation.md#heat-kernel) has integral one. Boundedness of $g$ permits differentiation under the integral for $t>0$, proving $u_t=\Delta u$ and $|u|\le\|g\|_\infty$. Its [approximate identity](../../../fourier-analysis.md#approximate-identity) property gives $u(x,t)\to g(x)$, locally uniformly since $g$ is [continuous](../../../calculus.md#continuous-function). This bounded solution satisfies the required Gaussian-growth bound.

For [heat-equation uniqueness under Gaussian growth](../../../diffusion-equation.md#heat-equation-uniqueness-under-gaussian-growth), let $w$ be the difference of two solutions, so $w(x,0)=0$ and $|w|\le M_0e^{a|x|^2}$ on a finite time interval. Choose $b>a$ and a slab $0\le t\le\tau<1/(4b)$. The positive comparison solution

$$
\Phi_b(x,t)=\frac1{1-4bt}\exp\!\left(\frac{b|x|^2}{1-4bt}\right)
$$

satisfies $(\Phi_b)_t=\Delta\Phi_b$. For any $\varepsilon>0$, its faster spatial growth makes $|w|\le\varepsilon\Phi_b$ on a sufficiently large lateral cylinder boundary. At the initial boundary, $w=0$. The [heat equation maximum principle](../../../diffusion-equation.md#heat-equation-maximum-principle) applied to $\pm w-\varepsilon\Phi_b$ proves the same inequality inside. First allow the cylinder radius to increase, then let $\varepsilon\downarrow0$. Repeating these slabs proves uniqueness on every finite interval with the stated uniform growth bound. No spatial integrability of $g$ is required.

At time $T$, this is [Gaussian filtering](../../../computer-science.md#gaussian-blur) with covariance $2T I$, hence **$\sigma=\sqrt{2T}$ per coordinate**. With the angular-frequency [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$, the [Gaussian filtering Fourier multiplier](../../../computer-science.md#gaussian-filtering-fourier-multiplier) is

$$
\boxed{\widehat u(\xi,T)=e^{-T|\xi|^2}\widehat g(\xi)=e^{-\sigma^2|\xi|^2/2}\widehat g(\xi).}
$$

For merely bounded $g$, this identity is understood through [tempered distributions](../../../fourier-analysis.md#tempered-distribution). The multiplier leaves the zero frequency unchanged and attenuates large [frequencies](../../../physics.md#frequency) exponentially: it suppresses rapid noise fluctuations but blurs [image edges](../../../computer-science.md#image-edge). In cycles-per-length frequency $k$, the multiplier is $e^{-4\pi^2T|k|^2}$.

For the printed [Perona-Malik equation](../../../diffusion-equation.md#perona-malik-equation), retain the supplied conductance $c(s)=s e^{-s^2/(2\lambda^2)}$, which includes an extra factor $s$. In one dimension write $p=u_x$ and $F(p)=c(|p|)p=p|p|e^{-p^2/(2\lambda^2)}$. Then $u_t=F'(u_x)u_{xx}$, with

$$
F'(p)=|p|e^{-p^2/(2\lambda^2)}\left(2-\frac{p^2}{\lambda^2}\right)\quad(p\ne0),\qquad F'(0)=0.
$$

The [forward-backward threshold for gradient-weighted exponential diffusion](../../../diffusion-equation.md#forward-backward-threshold-for-gradient-weighted-exponential-diffusion) is therefore

$$
\boxed{0<|u_x|<\sqrt2\lambda:\ \text{forward diffusion};\quad |u_x|>\sqrt2\lambda:\ \text{backward diffusion}.}
$$

At $|u_x|=0$ and $\sqrt2\lambda$ the coefficient vanishes, giving degenerate diffusion. Increasing $\lambda$ increases the forward-diffusion range. Small nonzero slopes smooth, while large slopes formally sharpen; a negative coefficient produces short-wave growth and [ill-posedness](../../../partial-differential-equation.md#ill-posed-problem), so this is a dynamics explanation, not a general existence theorem for arbitrary data. Replacing the printed conductance by $e^{-s^2/(2\lambda^2)}$ would give threshold $\lambda$, but that is a different equation.

The [four-neighbour mean expansion](../../../finite-difference.md#four-neighbour-mean-expansion) follows by [Taylor expansion](../../../calculus.md#taylor-expansion): opposing first and third [derivatives](../../../calculus.md#derivative) cancel, so

$$
\operatorname{mean}_h(u)(x)=u(x)+\frac{h^2}{4}\Delta u(x)+\frac{h^4}{48}\bigl(u_{xxxx}(x)+u_{yyyy}(x)\bigr)+O(h^6).
$$

If $u(x_0)=\operatorname{mean}_h(u)(x_0)$ for every sufficiently small $h$, division by $h^2$ and passage to the [limit](../../../calculus.md#limit-of-a-function) give **$\Delta u(x_0)=0$**. This is a pointwise conclusion; it does not assert harmonicity in a whole neighbourhood.

For the area [median](../../../probability-theory.md#median) over the disk, the [disk-median curvature expansion](../../../computer-science.md#disk-median-curvature-expansion), at a point where $|\nabla u|\ne0$, is

$$
\operatorname{median}_{B_h(x_0)}u=u(x_0)+\frac{h^2}{6}\left(\Delta u-\frac{\nabla u^T(D^2u)\nabla u}{|\nabla u|^2}\right)(x_0)+o(h^2).
$$

Consequently the analogous [median](../../../probability-theory.md#median) fixed-point condition yields

$$
\boxed{\Delta u(x_0)-\frac{\nabla u(x_0)^T(D^2u(x_0))\nabla u(x_0)}{|\nabla u(x_0)|^2}
=|\nabla u(x_0)|\operatorname{div}\!\left(\frac{\nabla u}{|\nabla u|}\right)(x_0)=0.}
$$

This is the vanishing of the [level-line curvature](../../../differential-geometry.md#level-line-curvature) at $x_0$: to second order the level line is straight there. It need not be a straight segment. For example $u(x,y)=y+x^3$ has zero disk [median](../../../probability-theory.md#median) at the origin for every radius, by odd symmetry, but its zero level line is the cubic $y=-x^3$. Vanishing [curvature](../../../differential-geometry.md#curvature) on an entire connected regular level arc would force that arc to be straight. The factor $1/6$ is for the disk's uniform area measure; a circle-boundary [median](../../../probability-theory.md#median) has a different scale factor, while producing the same zero-curvature equation.

## 4

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

An [image segmentation](../../../computer-science.md#image-segmentation) separates an observed [image signal](../../../computer-science.md#image-signal) into regions that are smooth within themselves and separated by meaningful [image edges](../../../computer-science.md#image-edge). Pure [image smoothing](../../../computer-science.md#image-smoothing) blurs the very transitions that ought to define these regions. The [Mumford–Shah segmentation model](../../../computer-science.md#mumford-shah-functional) instead chooses the reconstruction and its discontinuity set together. For a bounded planar [Lipschitz domain](../../../real-analysis.md#lipschitz-domain) and bounded grey-value data $g$, one standard normalization is

$$
E(u,K)=\int_{\Omega\setminus K}(u-g)^2\,dx+\alpha\int_{\Omega\setminus K}|\nabla u|^2\,dx+\beta\mathcal H^1(K),\qquad\alpha,\beta>0.
$$

Here $K$ is the relatively closed edge set and $u\in H^1(\Omega\setminus K)$ can have different traces on its two sides. The first term is [quadratic fidelity](../../../inverse-problem.md#quadratic-fidelity), the second penalizes variation within regions, and the [Hausdorff measure](../../../measure-theory.md#hausdorff-measure) term charges total edge length. It balances fitting, denoising and economical region geometry. The model was developed by David Mumford and Jayant Shah; their [1989 paper](https://www.dam.brown.edu/people/mumford/vision/papers/1989c--Mumford-Shah-Wiley.pdf) formulates this joint variational approach.

All three terms matter. Without fidelity, a constant reconstruction with no edge has zero energy. Without the [gradient](../../../calculus.md#gradient) term, smooth data can be fitted exactly with no edge penalty. Without the length term, fine partitions with nearly constant region means can drive fidelity arbitrarily low while creating excessive boundaries. This is [segmentation overfitting without an edge penalty](../../../computer-science.md#segmentation-overfitting-without-an-edge-penalty). Increasing $\alpha$ favors flatter regions; increasing $\beta$ makes extra boundaries more expensive and can remove small features. These parameter effects describe a balance, not a guaranteed monotone evolution of every individual boundary.

For fixed $K$, varying $u$ gives the [fixed-edge Euler-Lagrange equation for Mumford–Shah](../../../computer-science.md#fixed-edge-euler-lagrange-equation-for-mumford-shah):

$$
u-\alpha\Delta u=g\quad\text{in each region},\qquad\partial_nu=0\quad\text{on free region boundaries and the unconstrained outer boundary}.
$$

The boundary condition is a separate one-sided [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) on each side of an edge, not [continuity](../../../calculus.md#continuous-function) of $u$ across it. The fidelity makes this fixed-edge problem [strictly convex](../../../real-analysis.md#strictly-convex-function), so its weak solution is unique by the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem). Optimizing the edge set remains a different geometric problem. The [nonconvexity of Mumford–Shah segmentation](../../../computer-science.md#nonconvexity-of-mumford-shah-segmentation) prevents a general uniqueness assertion or a guarantee that a numerical [stationary point](../../../calculus-of-variations.md#stationary-point) is globally optimal.

The [piecewise-constant Mumford–Shah problem](../../../computer-science.md#piecewise-constant-mumford-shah-problem) imposes $u=c_i$ on regions $E_i$. It minimizes

$$
\sum_i\int_{E_i}(c_i-g)^2\,dx+\frac\beta2\sum_i\operatorname{Per}(E_i;\Omega).
$$

The factor $1/2$ counts each shared internal boundary once. The [region means in piecewise-constant segmentation](../../../computer-science.md#region-means-in-piecewise-constant-segmentation) give $c_i=|E_i|^{-1}\int_{E_i}g$, provided $|E_i|>0$. Thus the remaining optimization concerns the partition. For a smooth interface between $i$ and $j$, moving it in the normal pointing out of $i$ changes fidelity by $[(c_i-g)^2-(c_j-g)^2]$ per unit displacement, while length changes by its [curvature](../../../differential-geometry.md#curvature) $\kappa$. The resulting [segmentation interface curvature balance](../../../computer-science.md#segmentation-interface-curvature-balance) is

$$
\beta\kappa=(c_j-g)^2-(c_i-g)^2.
$$

With equal isotropic interface costs, three freely meeting smooth edges satisfy the [triple-junction angle in isotropic segmentation](../../../computer-science.md#triple-junction-angle-in-isotropic-segmentation): force balance of their unit tangents gives angles of $120$ degrees. These are local stationarity conditions on regular interfaces, not a description of every singular edge configuration.

A simple [piecewise-constant segmentation contrast threshold](../../../computer-science.md#piecewise-constant-segmentation-contrast-threshold) explains why small objects can disappear. On a domain of area $A$, suppose two constant intensities differ by $d$, occupying areas $a$ and $A-a$ with internal boundary length $L$. Keeping that boundary fits the data exactly and costs $\beta L$. Merging both regions costs the within-region squared error $a(A-a)d^2/A$. Among these two candidates, splitting wins precisely when $\beta L<a(A-a)d^2/A$. Other partitions may beat either candidate, so this is not a universal global segmentation formula.

<a id="4/image-one-region-and-two-region-reconstructions-balance-contrast-fitting-against-interface-length"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64-segmentation-candidates.png)

**[Figure 1](#4/image-one-region-and-two-region-reconstructions-balance-contrast-fitting-against-interface-length). One-region and two-region reconstructions balance contrast fitting against interface length**.

This original synthetic example compares those two candidate geometries using their least-squares means. It illustrates the edge cost; it does not claim to compute the globally optimal [Mumford–Shah segmentation](../../../computer-science.md#mumford-shah-functional).

Existence is cleanly stated in the relaxed [SBV space](../../../inverse-problem.md#special-bounded-variation-space) formulation:

$$
E(u)=\int_\Omega(u-g)^2\,dx+\alpha\int_\Omega|\nabla u|^2\,dx+\beta\mathcal H^1(J_u),
$$

where $J_u$ is the [jump set of a bounded-variation function](../../../inverse-problem.md#jump-set-of-a-bounded-variation-function) and the [Cantor part of a bounded-variation derivative](../../../inverse-problem.md#cantor-part-of-a-bounded-variation-derivative) is absent. Clip a minimizing sequence to the bounded data range: this cannot increase fidelity, [gradient](../../../calculus.md#gradient) energy or jump length. Its values are uniformly bounded, its [gradients](../../../calculus.md#gradient) bounded in $L^2$, and its jump lengths bounded. The [SBV compactness theorem](../../../inverse-problem.md#sbv-compactness-theorem) supplies an $L^1$-convergent subsequence staying in the special class; bounded values also give strong $L^2$ convergence. The fidelity then converges, while [gradient](../../../calculus.md#gradient) energy and jump length are [lower semicontinuous](../../../calculus.md#lower-semicontinuity). The [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations) produces a [minimizer](../../../analysis.md#global-minimizer). The [essential closedness of Mumford–Shah jump sets](../../../computer-science.md#essential-closedness-of-mumford-shah-jump-sets) is the additional regularity result connecting this relaxed [minimizer](../../../analysis.md#global-minimizer) to a closed-edge formulation; existence in $SBV$ alone does not assert that every edge set is smooth.

A practical [continuous](../../../calculus.md#continuous-function) approximation is the [Ambrosio–Tortorelli approximation](../../../computer-science.md#ambrosio-tortorelli-approximation), introduced in [Ambrosio and Tortorelli's 1990 paper](https://onlinelibrary.wiley.com/doi/10.1002/cpa.3160430805). An auxiliary field $v\in[0,1]$ is near one in regions and near zero at edges. One normalized energy is

$$
E_\varepsilon(u,v)=\int_\Omega(u-g)^2+\alpha(v^2+\eta_\varepsilon)|\nabla u|^2
+\beta\left(\varepsilon|\nabla v|^2+\frac{(1-v)^2}{4\varepsilon}\right)\,dx,
\qquad0<\eta_\varepsilon=o(\varepsilon).
$$

The edge field weakens smoothing across a narrow transition, and its own energy approximates interface length. The [Gamma-convergence](../../../calculus-of-variations.md#gamma-convergence) result, together with the required compactness, relates global minimizing sequences to the limiting segmentation energy; it does not make the finite-parameter problem jointly [convex](../../../real-analysis.md#convex-function). Alternating the two fields solves quadratic elliptic subproblems, but initialization and stopping can affect which local stationary configuration is found. The strengths of the model are joint denoising and segmentation, sharp transitions and a geometric cost. Limitations include competing local minima, sensitivity to scale parameters, loss of fine texture, and boundaries driven by intensity rather than semantic object identity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
