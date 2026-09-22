# Little Picard theorem

↑ **Parent:** [Picard theorem](picard-theorem.md)

Every nonconstant [entire function](entire-function.md) takes every complex value with at most one exception. Equivalently, its [image](image-of-a-function.md) is either $\mathbb C$ or $\mathbb C\setminus\{a\}$ for one complex number $a$. The hypothesis of being nonconstant matters: a [constant function](constant-function.md) has only one value. The [Little Picard theorem](little-picard-theorem.md) guarantees existence of [preimages](preimage.md), without requiring infinitely many [preimages](preimage.md) for each attained value. [Terence Tao, Math 246A Notes 4 (2016), Theorem 56](https://terrytao.wordpress.com/2016/10/11/math-246a-notes-4-singularities-of-holomorphic-functions/)

For a nonconstant [polynomial](polynomial-split.md) $p$, the [fundamental theorem of algebra](fundamental-theorem-of-algebra.md) applied to $p(z)-w$ supplies a [preimage](preimage.md) for every $w\in\mathbb C$. The [complex exponential function](complex-exponential-function.md) has precisely one [omitted value](omitted-value.md), zero, as the explicit formula for its [preimages](preimage.md) shows. In contrast, the [complex sine function](complex-sine-function.md) has no [omitted value](omitted-value.md). To solve $\sin z=w$, set $u=e^{iz}$ and rearrange to the [quadratic equation](quadratic-equation.md)

$$
u^2-2iwu-1=0.
$$

Its roots have product $-1$, so they are nonzero. Every such root has a [preimage](preimage.md) under the [complex exponential function](complex-exponential-function.md), giving a solution for $z$. Adding $2\pi k$ supplies further solutions by the [periodicity of the complex sine](periodicity-of-the-complex-sine.md).

The force of the [Little Picard theorem](little-picard-theorem.md) is that it applies to every nonconstant [entire function](entire-function.md), without an explicit formula. The [Liouville theorem](liouville-theorem.md) already gives a [dense image of a nonconstant entire function](dense-image-of-a-nonconstant-entire-function.md), but a [dense subset](dense-set.md) could still leave out many individual points. The [Little Picard theorem](little-picard-theorem.md) limits these missing points to one. In particular, establishing two [omitted values](omitted-value.md) proves that an [entire function](entire-function.md) is constant.

For a nonconstant [meromorphic function](meromorphic-function.md) on the [complex plane](complex-plane.md), the corresponding bound is two [omitted values](omitted-value.md) in the [Riemann sphere](riemann-sphere.md) $\mathbb C\cup\{\infty\}$, where [poles](pole.md) take the value infinity. [Picard, Mémoire sur les fonctions entières (1880), section 7, pp. 152-153](https://numdam.org/articles/10.24033/asens.187/) For example,

$$
m(z)=\frac1{1-e^z}
$$

omits zero and one, and has [poles](pole.md) at $2\pi i k$ for $k\in\mathbb Z$. Every other finite value $w$ is attained by solving $e^z=1-1/w$. For an [entire function](entire-function.md), infinity is already an [omitted value](omitted-value.md) in the [Riemann sphere](riemann-sphere.md), leaving at most one additional finite [omitted value](omitted-value.md).

Proof outline: use the version of [Montel's theorem](montel-s-theorem.md) for two fixed finite [omitted values](omitted-value.md). [Tao, Math 246A Notes 4, Exercise 58](https://terrytao.wordpress.com/2016/10/11/math-246a-notes-4-singularities-of-holomorphic-functions/) It makes the rescaled [holomorphic functions](holomorphic-function.md) $g_n(\zeta)=f(a+n\zeta)$ a [normal family](normal-family.md) on the [unit disc](unit-disc.md). The fixed value $g_n(0)=f(a)$ gives [pointwise anchoring of a holomorphic normal family](pointwise-anchoring-of-a-holomorphic-normal-family.md), hence a subsequence with a finite [holomorphic function](holomorphic-function.md) as its [locally uniform convergence](locally-uniform-convergence.md) limit. The [Cauchy integral formula](cauchy-integral-formula.md) bounds its [derivatives](derivative.md) at zero, whereas $g_n'(0)=nf'(a)$. Consequently $f'(a)=0$; arbitrary $a$ makes $f$ constant.

**Table of contents**

- [Great Picard theorem](great-picard-theorem.md)

## ↑ Ancestors (8)

1. [Picard theorem](picard-theorem.md)
2. [Entire function](entire-function.md)
3. [Holomorphic function](holomorphic-function.md)
4. [Complex analysis](complex-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Entire function](entire-function.md)
- [Great Picard theorem](great-picard-theorem.md)
- [Holomorphic map from the complex plane to a one-dimensional complex torus](holomorphic-map-from-the-complex-plane-to-a-one-dimensional-complex-torus.md)
- [Little Picard theorem](little-picard-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-10/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/23f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/23f/solution.md)
- [Picard theorem](picard-theorem.md)
- [Plane domain with two omitted points is hyperbolic](plane-domain-with-two-omitted-points-is-hyperbolic.md)
