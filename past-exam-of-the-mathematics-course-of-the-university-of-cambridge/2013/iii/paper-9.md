# Paper 9

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_9.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_9.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a unit direction $e$, let $T_\delta(a,e)$ be a length-one [Kakeya tube](../../../combinatorics.md#kakeya-tube) with transverse radius $\delta$, centered at $a$, and define the [Kakeya maximal function](../../../fourier-analysis.md#kakeya-maximal-function) by

$$
\mathcal K_\delta f(e)=\sup_a\frac1{|T_\delta(a,e)|}\int_{T_\delta(a,e)}|f(x)|\,dx.
$$

Using normalized surface measure on the direction sphere, the [Kakeya maximal conjecture](../../../fourier-analysis.md#kakeya-maximal-conjecture) is the following family of estimates, in the formulation relevant to this paper:

$$
\boxed{\|\mathcal K_\delta f\|_{L^n(S^{n-1})}
\le C_{n,\varepsilon}\delta^{-\varepsilon}\|f\|_{L^n(\mathbb R^n)}
\quad(0<\delta<1,\ \varepsilon>0).}
$$

The constant is independent of $\delta$ and $f$. Replacing round [Kakeya tubes](../../../combinatorics.md#kakeya-tube) by comparable rectangular tubes changes only dimensional constants.

A bounded [Kakeya set](../../../combinatorics.md#kakeya-set) contains a unit line segment in every direction. The [Kakeya Minkowski dimension conjecture](../../../combinatorics.md#kakeya-minkowski-dimension-conjecture) says that every such set has full [Minkowski dimension](../../../geometry-and-topology.md#box-counting-dimension) $n$. The maximal estimate in fact gives full lower as well as upper [Minkowski dimension](../../../geometry-and-topology.md#box-counting-dimension).

To prove that implication, let $E_\delta=\{x:\operatorname{dist}(x,E)<\delta\}$. Each unit segment in $E$ has a thinner tube contained in $E_\delta$, so $\mathcal K_{c\delta}\mathbf1_{E_\delta}(e)\ge1$ for every $e$, with a fixed dimensional $c>0$. Apply the maximal estimate to this [indicator function](../../../measure-theory.md#indicator-function):

$$
1\lesssim C_{n,\varepsilon}\delta^{-\varepsilon}|E_\delta|^{1/n},
\qquad |E_\delta|\gtrsim_{n,\varepsilon}\delta^{n\varepsilon}.
$$

If $N_\delta(E)$ is the smallest number of radius-$\delta$ balls covering $E$, that cover, enlarged by a fixed factor, covers $E_\delta$. Thus $|E_\delta|\lesssim_n\delta^n N_\delta(E)$ and

$$
N_\delta(E)\gtrsim_{n,\varepsilon}\delta^{-n+n\varepsilon}.
$$

Taking the lower limit of $\log N_\delta(E)/\log(1/\delta)$ and then letting $\varepsilon\downarrow0$ gives lower [Minkowski dimension](../../../geometry-and-topology.md#box-counting-dimension) at least $n$. Bounded subsets of $\mathbb R^n$ have upper [Minkowski dimension](../../../geometry-and-topology.md#box-counting-dimension) at most $n$. Consequently **both dimensions equal $n$**, which proves the requested implication.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

It is enough to prove the stronger planar [Kakeya maximal function](../../../fourier-analysis.md#kakeya-maximal-function) bound

$$
\boxed{\|\mathcal K_\delta f\|_{L^2(S^1)}
\lesssim\sqrt{\log(2/\delta)}\,\|f\|_{L^2(\mathbb R^2)}.}
$$

We first work with a $\delta$-separated net of unoriented directions $e_1,\ldots,e_M$, with $M\asymp\delta^{-1}$. Write $\alpha_{ij}$ for angular distance modulo $\pi$. Choose arbitrary length-one, width-$\delta$ rectangles $T_j$ in these directions. The permitted rectangle intersection fact is

$$
|T_i\cap T_j|\lesssim\min\left(\delta,\frac{\delta^2}{\alpha_{ij}}\right)
\lesssim\frac{\delta^2}{\delta+\alpha_{ij}}.
$$

The first alternative includes parallel rectangles. Their locations are arbitrary; only separation of their directions matters.

Define $Af(j)=\delta^{-1}\int_{T_j}f$, and put $\|a\|_{\ell^2_\delta}^2=\delta\sum_j|a_j|^2$. With these weights the [adjoint operator](../../../hilbert-space.md#adjoint-operator) is $A^*a=\sum_j a_j\mathbf1_{T_j}$. Since a separated angular net has only a bounded number of directions at each distance scale $k\delta$ from $e_i$, its overlap matrix satisfies

$$
\sum_j|T_i\cap T_j|
\lesssim\delta+\sum_{k=1}^{O(\delta^{-1})}\frac{\delta}{k}
\lesssim\delta\log(2/\delta).
$$

The diagonal term is of size $\delta$. Using $|a_i a_j|\le(|a_i|^2+|a_j|^2)/2$ and symmetry gives the [Schur test](../../../topological-vector-space.md#schur-test) estimate

$$
\begin{aligned}
\|A^*a\|_2^2
&\le\sum_{i,j}|a_i a_j|\,|T_i\cap T_j|\\
&\lesssim\delta\log(2/\delta)\sum_i|a_i|^2
=\log(2/\delta)\|a\|_{\ell^2_\delta}^2.
\end{aligned}
$$

By [duality of Lp spaces](../../../continuous-dual-space.md#duality-of-lp-spaces), $\|Af\|_{\ell^2_\delta}\lesssim\sqrt{\log(2/\delta)}\|f\|_2$. This is uniform over every choice of the translated rectangles. For each direction choose a rectangle approaching the supremum for $|f|$, then take the limit. That gives the same estimate for the discretized [Kakeya maximal function](../../../fourier-analysis.md#kakeya-maximal-function).

To recover all directions, partition the direction circle into arcs of length comparable to $\delta$, each with a net direction. A tube in an arc is contained in a rectangle in its net direction with width $C\delta$ and length at most two. A bounded subdivision in the length direction reduces this to the same averaging operators; the wider tubes obey the same overlap estimate with fixed-factor changes. Therefore

$$
\int_{S^1}|\mathcal K_\delta f(e)|^2\,de
\lesssim\delta\sum_j|\mathcal K_{C\delta}^{\mathrm{net}}f(e_j)|^2
\lesssim\log(2/\delta)\|f\|_2^2.
$$

Finally $\sqrt{\log(2/\delta)}\le C_\varepsilon\delta^{-\varepsilon}$ for every $\varepsilon>0$. **The [planar Kakeya maximal estimate](../../../fourier-analysis.md#planar-kakeya-maximal-estimate) therefore has the required arbitrary small power loss.**

## 2

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat\nu(\xi)=\int e^{-ix\cdot\xi}\,d\nu(x)$ throughout this question. The decay assumption implies square integrability, since [polar coordinates](../../../calculus.md#polar-coordinates) give

$$
\int_{\mathbb R^2}|\widehat\mu(\xi)|^2\,d\xi
\lesssim\int_0^\infty\frac{r}{(1+r^{1+\epsilon})^2}\,dr<\infty.
$$

Near zero the integrand is bounded by $r$, and at infinity it is bounded by $r^{-1-2\epsilon}$. The positive $\epsilon$ is what makes the latter integrable.

By the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem), there is a function $g\in L^2(\mathbb R^2)$ whose [Fourier transform](../../../analysis.md#fourier-transform) is $\widehat\mu$. It is the density of $\mu$ with respect to [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). To justify this step rather than assume a density, for every [Schwartz function](../../../fourier-analysis.md#schwartz-function) $\varphi$, [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\int\varphi\,d\mu
=(2\pi)^{-2}\int\widehat\varphi(-\xi)\widehat\mu(\xi)\,d\xi
=\int\varphi(x)g(x)\,dx.
$$

The [finite measure](../../../measure-theory.md#finite-measure) and the locally integrable function thus define the same [tempered distribution](../../../fourier-analysis.md#tempered-distribution), so they agree as measures: $d\mu=g\,dx$. In particular $g\ge0$ almost everywhere and $\int g=\mu(\mathbb R^2)<\infty$. This is the [L2 density from a square-integrable Fourier transform](../../../fourier-analysis.md#l2-density-from-a-square-integrable-fourier-transform) principle.

For $f\in L^\infty(\mu)$, the density of $f\,d\mu$ is $fg$. The inequality $|f|\le\|f\|_{L^\infty(\mu)}$ holds wherever $g>0$, apart from a [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) zero set, so

$$
\|fg\|_2\le\|f\|_{L^\infty(\mu)}\|g\|_2.
$$

A second application of the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) yields the explicit bound

$$
\boxed{\|\widehat{f\,d\mu}\|_2
=(2\pi)\|fg\|_2
\le\|\widehat\mu\|_2\,\|f\|_{L^\infty(\mu)}.}
$$

The implicit constant in the requested estimate may depend on the measure and its Fourier-decay bound, but is independent of $f$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Parametrize the [unit circle](../../../complex-analysis.md#complex-unit-circle) by $\omega(\theta)=(\cos\theta,\sin\theta)$, with $-\pi\le\theta<\pi$ and $d\sigma=d\theta/(2\pi)$. Extract the constant phase at $\omega(0)$:

$$
e^{i\xi_1}\widehat{\psi\,d\sigma}(\xi)
=\frac1{2\pi}\int\psi(\omega(\theta))
 e^{-i[\xi_1(\cos\theta-1)+\xi_2\sin\theta]}\,d\theta.
$$

On the support, $|\theta|\le2\delta/C$. The frequency rectangle and the elementary bounds $|1-\cos\theta|\le\theta^2/2$, $|\sin\theta|\le|\theta|$ imply

$$
|\xi_1(\cos\theta-1)+\xi_2\sin\theta|
\le\frac2{C^2}+\frac2C.
$$

Choose the fixed constant $C$ large enough that this is less than $\pi/3$. Every phase then has real part at least $1/2$. Nonnegativity of $\psi$ prevents cancellation after this phase rotation, while its central plateau gives $\int\psi\,d\sigma\ge\delta/(\pi C)$. Hence the [Fourier transform](../../../analysis.md#fourier-transform) satisfies

$$
\boxed{|\widehat{\psi\,d\sigma}(\xi)|
\ge\operatorname{Re}\!\left(e^{i\xi_1}\widehat{\psi\,d\sigma}(\xi)\right)
\ge\frac12\int\psi\,d\sigma
\ge\frac{\delta}{2\pi C}.}
$$

This is the [circle cap Fourier lower bound](../../../fourier-analysis.md#circle-cap-fourier-lower-bound). No upper bound on the values of $\psi$ is needed here; the support, plateau and nonnegativity suffice. The long radial scale $\delta^{-2}$ comes from the quadratic term $\cos\theta-1$, whereas the transverse scale $\delta^{-1}$ comes from the linear term $\sin\theta$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write $R_j$ for the rectangles, $x_j$ for their centers and $e_j$ for their long-axis directions. For the finite exponent $p$ in the displayed estimate, take smooth rotated cap functions $\psi_j$, with $0\le\psi_j\le1$, equal to one on angular distance at most $\delta/C$ from $e_j$ and supported within $2\delta/C$. Choose $C$ sufficiently large once and for all. The direction separation makes these cap supports disjoint, and $\int|\psi_j|^p\,d\sigma\lesssim\delta$.

Define

$$
f_j(\omega)=e^{ix_j\cdot\omega}\psi_j(\omega),\qquad
h_j(x)=\widehat{f_j\,d\sigma}(x)
=\widehat{\psi_j\,d\sigma}(x-x_j).
$$

The [Fourier modulation and translation identity](../../../analysis.md#modulation-property-of-the-fourier-transform) gives the second equality. Rotating the [circle cap Fourier lower bound](../../../fourier-analysis.md#circle-cap-fourier-lower-bound) then gives **$|h_j(x)|\gtrsim\delta$ on $R_j$**. The half-side lengths of $R_j$ are no larger than the two frequency bounds used in part (b).

Let $\varepsilon_j$ be independent [Rademacher random variables](../../../probability-theory.md#rademacher-distribution). Because the input cap supports are disjoint, for every choice of signs

$$
\left\|\sum_j\varepsilon_j f_j\right\|_{L^p(\sigma)}^p
=\sum_j\|\psi_j\|_{L^p(\sigma)}^p\lesssim M\delta,
$$

where $M=\#\mathcal R$. Apply the assumed [Fourier extension estimate](../../../fourier-analysis.md#fourier-extension-estimate) to the sum. Average over signs and use the [Khintchine inequality](../../../fourier-analysis.md#khintchine-inequality) pointwise, followed by the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem):

$$
\int_{\mathbb R^2}\left(\sum_j|h_j(x)|^2\right)^{p/2}\,dx
\lesssim_p\mathbb E\left\|\sum_j\varepsilon_jh_j\right\|_p^p
\lesssim_p M\delta.
$$

There is no requirement that the spatial rectangles be disjoint; disjointness is used only for the input caps on the [unit circle](../../../complex-analysis.md#complex-unit-circle). Their spatial overlaps are precisely what the square function measures. The cap lower bounds now imply

$$
\delta^p\int\left(\sum_j\mathbf1_{R_j}\right)^{p/2}
\lesssim_p M\delta.
$$

Since each rectangle has area $\delta^{-3}$, the [restriction-to-rectangle overlap principle](../../../fourier-analysis.md#restriction-to-rectangle-overlap-principle) gives

$$
\boxed{\int\left(\sum_{R\in\mathcal R}\mathbf1_R\right)^{p/2}
\lesssim_p M\delta^{1-p}
=\delta^{4-p}\sum_{R\in\mathcal R}|R|.}
$$

The constants are independent of $\delta$, the centers and the collection. The finite-$p$ interpretation is the one for which the printed power integral is defined. A single cap also shows that the assumed diagonal [Fourier extension estimate](../../../fourier-analysis.md#fourier-extension-estimate) can hold only for $p\ge4$: its output contributes at least $\delta^{p-3}$ to the $p$th-power [norm](../../../functional-analysis.md#norm), whereas its input contributes at most a constant times $\delta$.

## 3

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Set $m=\lceil p/100\rceil$ and $d=m-1$, so that $d<p/100<p$. The [dimension of a bounded-total-degree polynomial space](../../../polynomial.md#dimension-of-a-bounded-total-degree-polynomial-space) in $n$ variables over $\mathbb F_p$ is $\binom{n+d}{n}$. If $\#N$ were smaller than this dimension, evaluation at the points of $N$ would impose fewer homogeneous linear conditions than unknown coefficients. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) would give a nonzero [multivariate polynomial](../../../polynomial.md#multivariate-polynomial) $P$ of [total degree](../../../polynomial.md#total-degree-of-a-polynomial) at most $d$, vanishing on $N$.

For every $x$, select one of the promised rich [affine lines in a vector space](../../../vector-space.md#affine-line-in-a-vector-space) through $x$, and write it as $\ell=\{a+tv:t\in\mathbb F_p\}$ with $v\ne0$. The [polynomial restriction to a line](../../../polynomial.md#polynomial-restriction-to-a-line) $Q(t)=P(a+tv)$ has degree at most $d$, and at least $m=d+1$ distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) from $N\cap\ell$. By the [root bound for a polynomial](../../../polynomial.md#lagrange-root-bound-over-a-field), **$Q$ is identically zero**, so $P(x)=0$. Since this works for every $x$, $P$ vanishes at all $p^n$ points of $\mathbb F_p^n$.

The [Schwartz-Zippel lemma](../../../combinatorics.md#schwartz-zippel-lemma) says that a nonzero [multivariate polynomial](../../../polynomial.md#multivariate-polynomial) of [total degree](../../../polynomial.md#total-degree-of-a-polynomial) $d$ has at most $d p^{n-1}$ zeros on this grid. Here $d<p$, so that count is strictly less than $p^n$, a contradiction. The distinction between a formal [polynomial](../../../polynomial.md) and its function on a [finite field](../../../algebra.md#finite-field) is crucial: our degree bound is what rules out a nonzero [polynomial](../../../polynomial.md) vanishing everywhere.

We have proved the stronger quantitative [rich line covering bound over a finite field](../../../combinatorics.md#rich-line-covering-bound-over-a-finite-field)

$$
\boxed{\#N\ge\binom{n+\lceil p/100\rceil-1}{n}
=\frac{(d+1)\cdots(d+n)}{n!}
\ge\frac{p^n}{100^n n!}.}
$$

Thus **$\#N\gtrsim_n p^n$**, as required. The implied constant may depend on the fixed dimension $n$. The very large numerical lower bound on $p$ is more than this proof needs.

## 4

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a finite collection $\mathcal L$ of distinct [affine lines in a vector space](../../../vector-space.md#affine-line-in-a-vector-space) in $\mathbb R^n$, $n\ge2$, a [joint](../../../combinatorics.md#joint-of-a-line-collection) is a point incident to $n$ lines whose direction vectors are [linearly independent](../../../vector-space.md#linear-independence). The [joints theorem](../../../combinatorics.md#joints-theorem) asserts

$$
\boxed{\#J(\mathcal L)\lesssim_n(\#\mathcal L)^{n/(n-1)}.}
$$

In the customary three-dimensional formulation this is **$\#J\lesssim L^{3/2}$**, with three noncoplanar incident lines at every [joint](../../../combinatorics.md#joint-of-a-line-collection). We prove the general form, which includes that formulation.

Let $L=\#\mathcal L$ and $M=\#J$. The conclusion is immediate when $M=0$. Otherwise set $D=\lceil nM^{1/n}\rceil$. Suppose for contradiction that $M>LD$. Repeatedly delete any line incident to at most $D$ of the currently retained [joints](../../../combinatorics.md#joint-of-a-line-collection), deleting those [joints](../../../combinatorics.md#joint-of-a-line-collection) at the same time. Each deleted line loses at most $D$ current [joints](../../../combinatorics.md#joint-of-a-line-collection), so even deleting all $L$ lines could lose at most $LD<M$ [joints](../../../combinatorics.md#joint-of-a-line-collection). Therefore the process must stop with a nonempty set $J'$ and a line collection $\mathcal L'$ such that **each retained line contains more than $D$ retained [joints](../../../combinatorics.md#joint-of-a-line-collection)**. Every retained [joint](../../../combinatorics.md#joint-of-a-line-collection) still has its original $n$ independent incident lines: if any line through it had been deleted, the [joint](../../../combinatorics.md#joint-of-a-line-collection) would have been deleted too.

There is a nonzero [multivariate polynomial](../../../polynomial.md#multivariate-polynomial) of [total degree](../../../polynomial.md#total-degree-of-a-polynomial) at most $D$ vanishing on $J'$, because

$$
\binom{D+n}{n}\ge\frac{D^n}{n!}
\ge\frac{n^n}{n!}M>M\ge\#J'.
$$

Choose such a [polynomial](../../../polynomial.md) $P$ of smallest possible [total degree](../../../polynomial.md#total-degree-of-a-polynomial) $d\le D$. This is an application of the [polynomial method in combinatorics](../../../combinatorics.md#polynomial-method-in-combinatorics). Every line of $\mathcal L'$ contains more than $D\ge d$ [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) of its [polynomial restriction to a line](../../../polynomial.md#polynomial-restriction-to-a-line), so $P$ vanishes identically on every such line.

At a retained [joint](../../../combinatorics.md#joint-of-a-line-collection) $x$, differentiating along each of its independent line directions $v_1,\ldots,v_n$ gives $v_i\cdot\nabla P(x)=0$. Their [linear independence](../../../vector-space.md#linear-independence) therefore forces $\nabla P(x)=0$. Each [partial derivative](../../../calculus.md#partial-derivative) of $P$ vanishes on all of $J'$ and has smaller [total degree](../../../polynomial.md#total-degree-of-a-polynomial). Minimality of $d$ forces every [partial derivative](../../../calculus.md#partial-derivative) to be the zero [polynomial](../../../polynomial.md). Over the real numbers, a [polynomial](../../../polynomial.md) with all [partial derivatives](../../../calculus.md#partial-derivative) zero is constant; a nonzero constant cannot vanish on the nonempty $J'$. This is the required contradiction.

It follows that $M\le LD$. Since $D\le(n+1)M^{1/n}$ for $M\ge1$,

$$
M^{(n-1)/n}\le(n+1)L,
\qquad
\boxed{M\le((n+1)L)^{n/(n-1)}.}
$$

This proves the [joints theorem](../../../combinatorics.md#joints-theorem) by the [pruning and minimal-degree polynomial argument](../../../combinatorics.md#pruning-and-minimal-degree-polynomial-argument).

The exponent is sharp. Take all axis-parallel lines passing through the grid $\{1,\ldots,m\}^n$. There are $n m^{n-1}$ distinct lines and $m^n$ [joints](../../../combinatorics.md#joint-of-a-line-collection); the coordinate directions span $\mathbb R^n$ at every grid point. Thus no smaller power of the number of lines can bound all [joint](../../../combinatorics.md#joint-of-a-line-collection) configurations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
