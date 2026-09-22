<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [contraction semigroup](../../../../../../contraction-semigroup.md) on a [Banach space](../../../../../../banach-space-split.md) $X$ consists of bounded linear operators $S(t)$ with $S(0)=I$, $S(t+s)=S(t)S(s)$, $\|S(t)\|\leq1$, and $S(t)x\to x$ as $t\downarrow0$ for each $x\in X$. Its [infinitesimal generator of a semigroup](../../../../../../infinitesimal-generator-of-a-semigroup.md) is

$$
D(A)=\left\{x:\lim_{h\downarrow0}\frac{S(h)x-x}{h}\text{ exists in }X\right\},
\qquad
Ax=\lim_{h\downarrow0}\frac{S(h)x-x}{h}.
$$

For density, [Yosida averaging of a semigroup](../../../../../../yosida-averaging-of-a-semigroup.md) gives $x_h=h^{-1}\int_0^hS(s)x\,ds$. Taking the difference quotient of this [Bochner integral](../../../../../../bochner-integral.md) shows that $x_h\in D(A)$ and $Ax_h=(S(h)x-x)/h$. Strong continuity gives $x_h\to x$, so $D(A)$ is dense.

For closedness, the [semigroup restricted to its generator domain](../../../../../../semigroup-restricted-to-its-generator-domain.md) satisfies

$$
S(t)x-x=\int_0^tS(s)Ax\,ds\qquad(x\in D(A)).
$$

If $x_n\to x$ and $Ax_n\to y$, pass to the limit in this identity. After dividing by $t$, strong continuity gives $(S(t)x-x)/t\to y$. Hence $x\in D(A)$ and $Ax=y$. This proves [generator of a strongly continuous semigroup is closed and densely defined](../../../../../../generator-of-a-strongly-continuous-semigroup-is-closed-and-densely-defined.md).

The contraction form of the [Hille-Yosida theorem](../../../../../../hille-yosida-theorem.md) states that a linear operator $A$ generates a [contraction semigroup](../../../../../../contraction-semigroup.md) if and only if it is densely defined and closed, every real $\lambda>0$ lies in its [resolvent set](../../../../../../resolvent-set-of-an-operator.md), and

$$
\|(\lambda-A)^{-n}\|\leq\lambda^{-n}\qquad(n\geq1).
$$

Here the $n=1$ bound implies the others by taking powers of the same bounded [resolvent](../../../../../../resolvent-of-an-operator.md).

The [H1 space](../../../../../../h1-space.md) is $H^1(\mathbb R)=\{u\in L^2:u'\in L^2\}$ with [weak derivative](../../../../../../weak-derivative.md) $u'$ and squared norm $\|u\|_2^2+\|u'\|_2^2$. The displayed weighted space is the [one-dimensional harmonic oscillator form domain](../../../../../../one-dimensional-harmonic-oscillator-form-domain.md), with inner product

$$
\langle u,v\rangle_X=\int_{\mathbb R}u\bar v+u'\overline{v'}+x^2u\bar v\,dx.
$$

If $u_n$ is Cauchy in $X$, it converges in $H^1$ to $u$, and $xu_n$ converges in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) to some $w$. On each bounded interval, multiplication by $x$ is bounded, so $w=xu$ there. Thus $xu\in L^2$ and convergence holds in $X$, proving completeness and the [Hilbert space](../../../../../../hilbert-space-split.md) property. Equivalently this is closedness of the [multiplication operator](../../../../../../multiplication-operator.md) by $x$.

For the [Sobolev characterization by bounded difference quotients](../../../../../../sobolev-characterization-by-bounded-difference-quotients.md), if $f\in H^1$ then

$$
D_hf=\int_0^1f'(\cdot+\theta h)\,d\theta,
\qquad
\|D_hf\|_2\leq\|f'\|_2,
\qquad
D_hf\longrightarrow f'\text{ in }L^2.
$$

The last assertion uses continuity of [translation of a function](../../../../../../translation-of-a-function.md) in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). Conversely, if $f\in L^2$ and the quotients are uniformly bounded for $0<|h|<1$, take a weakly convergent subsequence as $h\to0$. For every [test function](../../../../../../test-function.md) $v$,

$$
\int D_hf\,v\,dx=\int f(x)\frac{v(x-h)-v(x)}h\,dx\longrightarrow-\int f v'\,dx.
$$

The weak limit is therefore the [weak derivative](../../../../../../weak-derivative.md) $f'\in L^2$. This proves the characterization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
