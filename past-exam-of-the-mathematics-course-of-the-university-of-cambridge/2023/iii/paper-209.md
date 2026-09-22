# Paper 209

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_209.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_209.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For a finite graph $\Lambda=(V,E)$ with [free boundary conditions](../../../statistical-physics.md#free-boundary-condition), write $\sigma_x=(\cos\theta_x,\sin\theta_x)\in S^1$. The ferromagnetic [O(2) model](../../../statistical-physics.md#xy-model) is

$$
d\mu_{\Lambda,\beta,h}(\theta)
=\frac1Z\exp\left\{\beta\sum_{xy\in E}\cos(\theta_x-\theta_y)
+h\sum_{x\in V}\cos\theta_x\right\}
\prod_{x\in V}\frac{d\theta_x}{2\pi}.
$$

The [Ginibre inequality](../../../statistical-physics.md#ginibre-inequality) says, in particular, that for $a,b\in\mathbb Z_{\geq0}^V$,

$$
\langle\cos(a\cdot\theta)\cos(b\cdot\theta)\rangle
\geq
\langle\cos(a\cdot\theta)\rangle
\langle\cos(b\cdot\theta)\rangle.
$$

For the proof, take two independent replicas $\theta,\theta'$ and write the covariance as one half of the expectation of

$$
\{\cos(a\cdot\theta)-\cos(a\cdot\theta')\}
\{\cos(b\cdot\theta)-\cos(b\cdot\theta')\}.
$$

Set $u=(\theta+\theta')/2$ and $v=(\theta-\theta')/2$. Product-to-sum identities turn each difference into $-2\sin(a\cdot u)\sin(a\cdot v)$, while every replicated interaction becomes

$$
\cos(\theta_x-\theta_y)+\cos(\theta'_x-\theta'_y)
=2\cos(u_x-u_y)\cos(v_x-v_y).
$$

Expand every exponential in a power series and then every cosine power into Fourier modes. Integration over each angle kills all unmatched modes. Because the couplings, field, and entries of $a,b$ are nonnegative, every surviving paired coefficient in the covariance is nonnegative. Their sum is therefore nonnegative, proving the inequality. The same replica expansion proves the usual product version.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Differentiate the finite-volume magnetization:

$$
\frac d{dh}\langle\sigma_x^1\rangle_{\Lambda,\beta,h}
=\sum_{y\in V}
\left\{
\langle\cos\theta_x\cos\theta_y\rangle
-\langle\cos\theta_x\rangle\langle\cos\theta_y\rangle
\right\}.
$$

Every summand is nonnegative by the [Ginibre inequality](../../../statistical-physics.md#ginibre-inequality) with $a=\mathbf1_x$ and $b=\mathbf1_y$. Hence the magnetization is nondecreasing for $h\geq0$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

At zero field the finite-volume law is invariant under the global rotation $\theta_z\mapsto\theta_z+\alpha$. Averaging $\cos(2\theta_x)$ over $\alpha$ gives zero. Reflection $\theta_z\mapsto-\theta_z$ likewise gives $\langle\sin\theta_y\rangle=0$. Thus

$$
\langle\cos(2\theta_x)-\sin(\theta_y)\rangle_{\Lambda,\beta,0}=0
$$

for every finite $\Lambda$ containing $x,y$, so its infinite-volume limit exists and equals zero.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Let the square contain the Euclidean ball of radius $R$, set $r_x=\max(1,\lVert x\rVert)$, and define the logarithmic cutoff

$$
\varphi_x=
\begin{cases}
1,&r_x=1,\\
\dfrac{\log(R/r_x)}{\log R},&1<r_x<R,\\
0,&r_x\geq R.
\end{cases}
$$

Then $\varphi_0=1$ and $\varphi=0$ on the boundary. On an edge at radius comparable to $r$, the [mean value theorem](../../../calculus.md#mean-value-theorem) gives $|\varphi_x-\varphi_y|\leq C/(r\log R)$. There are $O(r)$ edges in the annulus of radius $r$, hence the [discrete Dirichlet energy](../../../markov-process.md#discrete-dirichlet-energy) satisfies

$$
\sum_{xy\in\bar E}(\varphi_x-\varphi_y)^2
\leq\frac C{(\log R)^2}\sum_{r=1}^{R}\frac1r
\leq\frac C{\log R}\longrightarrow0.
$$

This logarithmic cutoff is the discrete manifestation of recurrence in two dimensions.

## 2

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $\Delta$ be the torus graph Laplacian and let $v:\Lambda_L\to\mathbb R^n$ have zero spatial mean. [Gaussian domination](../../../statistical-physics.md#gaussian-domination) states, in a standard normalization, that

$$
\frac{Z(v)}{Z(0)}
\leq
\exp\left\{\frac1{2\beta}(v,(-\Delta)^{-1}v)\right\}.
$$

Differentiating twice at zero gives the [infrared bound](../../../statistical-physics.md#infrared-bound): for every nonzero torus momentum $k$,

$$
\widehat G_L(k)
\leq\frac{n}{2\beta\,\varepsilon(k)},
\qquad
\varepsilon(k)=\sum_{j=1}^d(1-\cos k_j),
$$

up to the harmless normalization convention used for the Fourier transform and Hamiltonian.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The spin-length sum rule and Fourier inversion give

$$
1=\langle|\sigma_0|^2\rangle
=\frac1{|\Lambda_L|}\sum_k\widehat G_L(k).
$$

The zero mode contains the square of the field-directed magnetization, while the [infrared bound](../../../statistical-physics.md#infrared-bound) controls all nonzero modes. After $L\to\infty$ and then $h\downarrow0$,

$$
m(\beta)^2
\geq1-\frac{n}{2\beta}
\int_{[-\pi,\pi]^d}\frac{dk}{(2\pi)^d\,\varepsilon(k)}.
$$

Near zero, $\varepsilon(k)\asymp|k|^2$, so the integral is finite exactly when $d\geq3$. Choose $\beta_0$ larger than the resulting finite constant. Then for $\beta>\beta_0$ the right side is positive, and $m(\beta)\geq c>0$.

If $h\downarrow0$ before $L\to\infty$, every finite torus retains global $O(n)$ symmetry and its magnetization is zero. The reversed iterated limit is therefore zero. The order of limits is what permits [spontaneous magnetization](../../../statistical-physics.md#spontaneous-magnetization).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The field leaves rotations fixing its unit direction $e$ as symmetries. Consequently the expectation vector is parallel to $e$:

$$
\lim_{h\downarrow0}\lim_{L\to\infty}\langle\sigma_0\rangle_{\Lambda_L,\beta,h}
=m e.
$$

For any $u\in\mathbb R^n$, linearity therefore gives

$$
\boxed{\lim_{h\downarrow0}\lim_{L\to\infty}
\langle\sigma_0\cdot u\rangle_{\Lambda_L,\beta,h}
=m(e\cdot u).}
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $\vartheta$ be either permitted torus reflection and let $\Lambda_+$ be one reflected half. Under the product measure $\mu^{\otimes\Lambda_L}$, variables in the two open halves are independent and corresponding variables have the same law. For any $F$ depending on $\Lambda_+$,

$$
\int F\,\vartheta F\,d\mu^{\otimes\Lambda_L}
=\left|\int F\,d\mu^{\otimes\Lambda_+}\right|^2\geq0
$$

when the reflection has no fixed sites. If it fixes a layer of sites, condition on that layer; the same factorization gives a conditional square, whose expectation is nonnegative. This proves [reflection positivity](../../../statistical-physics.md#reflection-positivity) through sites. For an edge reflection the parity assumption makes the two halves pair exactly, so the first factorization applies there as well.

## 3

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In the one-dimensional zero-field [Ising model](../../../statistical-physics.md#ising-model), the bond variables $\tau_j=\sigma_j\sigma_{j+1}$ are independent and

$$
\mathbb E\tau_j=\frac{e^\beta-e^{-\beta}}{e^\beta+e^{-\beta}}=\tanh\beta.
$$

Since $\sigma_0\sigma_x=\prod_{j=0}^{x-1}\tau_j$ for $x>0$,

$$
\langle\sigma_0\sigma_x\rangle_{\beta,0}^{\mathbb Z}
=(\tanh\beta)^{|x|}
=e^{-c(\beta)|x|},
\qquad c(\beta)=-\log(\tanh\beta)>0.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

In a finite interval, the effect at the origin of a fixed boundary spin a distance $N$ away is bounded by its two-point correlation, $(\tanh\beta)^N$. With two boundaries,

$$
|\langle\sigma_0\rangle_{\Lambda_N,\beta,0}^{\pm}|
\leq2(\tanh\beta)^N\longrightarrow0.
$$

**Thus the plus and minus boundary limits coincide with the unique spin-flip-symmetric one-dimensional Gibbs state, and $\langle\sigma_0\rangle_{\beta,0}^{\mathbb Z,\pm}=0$ for every finite $\beta$.**

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The product $\sigma_0\sigma_1\cdots\sigma_{2022}$ contains $2023$ spins and changes sign under the global spin flip $\sigma\mapsto-\sigma$. By part ii, the infinite-volume plus state is spin-flip symmetric. Therefore

$$
\boxed{\langle\sigma_0\sigma_1\cdots\sigma_{2022}\rangle_{\beta,0}^{\mathbb Z,+}=0.}
$$

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Order the sites as $x_1<x_2<x_3<x_4$. Expressing spins through independent bond variables gives the [One-dimensional Ising correlation function](../../../statistical-physics.md#one-dimensional-ising-correlation-function)

$$
\langle\sigma_{x_1}\sigma_{x_2}\sigma_{x_3}\sigma_{x_4}\rangle_{\beta,0}^{\mathbb Z}
=(\tanh\beta)^{(x_2-x_1)+(x_4-x_3)}.
$$

If the minimum pairwise separation tends to infinity, both displayed gaps tend to infinity. Since $\tanh\beta<1$, the expectation tends to zero.

## 4

↑ **Parent:** [Paper 209](paper-209.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Under [plus boundary conditions](../../../statistical-physics.md#plus-boundary-condition), if $\sigma_0=-1$, the negative cluster containing the origin is surrounded by a [Peierls contour](../../../statistical-physics.md#peierls-contour) $\gamma$. Flipping all spins inside $\gamma$ is injective after $\gamma$ is specified and increases the Boltzmann weight by $e^{2\beta|\gamma|}$. Therefore

$$
\mathbb P_{\Lambda_L,\beta}^{+}(\sigma_0=-1)
\leq\sum_{\gamma\ni0}e^{-2\beta|\gamma|}.
$$

The number of length-$m$ contours surrounding the origin is at most $C m3^m$, so the sum tends to zero as $\beta\to\infty$, uniformly in $L$. For sufficiently large $\beta$ it is below $1/4$, and then

$$
\boxed{\langle\sigma_0\rangle_{\Lambda_L,\beta}^{+}
=1-2\mathbb P(\sigma_0=-1)\geq\frac12.}
$$

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Ferromagnetic monotonicity makes the plus-boundary expectation decrease as the finite volume grows, so

$$
\langle\sigma_0\rangle_{\beta,0}^{\mathbb Z^2,+}
=\lim_{L\to\infty}\langle\sigma_0\rangle_{\Lambda_L,\beta,0}^{+}
$$

exists. The uniform lower bound from part i passes to the limit, proving positive spontaneous magnetization at sufficiently large $\beta$.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The three-dimensional [Peierls argument](../../../probability-theory.md#peierls-argument) replaces planar contours by closed dual plaquette surfaces surrounding the negative cluster of the origin. A surface of area $m$ costs $e^{-2\beta m}$, and the number of connected surfaces of area $m$ containing a fixed nearby plaquette is at most $C^m$. Hence

$$
\mathbb P_{\beta}^{\mathbb Z^3,+}(\sigma_0=-1)
\leq\sum_{m\geq m_0}C^me^{-2\beta m}.
$$

This is below $1/2$ for sufficiently large $\beta$, so $\langle\sigma_0\rangle_{\beta,0}^{\mathbb Z^3,+}>0$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The on-site potential of the [Phi-four lattice model](../../../statistical-physics.md#phi-four-lattice-model) is

$$
V(s)=\frac g4s^4+\frac\nu2s^2,
\qquad V''(s)=3gs^2+\nu\geq\nu>0.
$$

In the [random-walk representation of a lattice-field covariance](../../../statistical-physics.md#random-walk-representation-of-a-lattice-field-covariance), $\langle\phi_x\phi_y\rangle$ is a Green function for a nearest-neighbour walk with a nonnegative environment-dependent killing rate bounded below by a positive constant depending on $\nu$. Dropping the quartic contribution can only decrease that killing, so

$$
0\leq\langle\phi_x\phi_y\rangle
\leq(-\Delta+\nu)^{-1}(x,y).
$$

The massive lattice Green function has the killed-walk expansion

$$
(-\Delta+\nu)^{-1}(x,y)
=\sum_{k\geq0}\frac1{2d+\nu}
\left(\frac{2d}{2d+\nu}\right)^k
\mathbb P_x(S_k=y),
$$

with normalization adjusted to the chosen Laplacian. Reaching $y$ requires at least $|x-y|_1$ steps, while the geometric survival factor is strictly below one. Summing the tail gives constants $C,c>0$ such that

$$
\boxed{|\langle\phi_x\phi_y\rangle|\leq Ce^{-c|x-y|_1}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
