<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A sufficient absolute constant is $\boxed{C=16}$. The proof is a [density increment](../../../../../density-increment.md) argument for a [cap set](../../../../../cap-set.md) over the [finite field](../../../../../finite-field.md) $\mathbb F_3$.

First work in $V=\mathbb F_3^d$, write $N=3^d$, and let $f=1_A$ be the [indicator function](../../../../../indicator-function.md) of a [cap set](../../../../../cap-set.md) of [subset density](../../../../../density-of-a-finite-subset.md) $\alpha>0$. All [expectations](../../../../../expected-value.md) below are uniform. In [characteristic](../../../../../characteristic-of-a-field.md) three, a solution of $x+y+z=0$ having two equal entries has all three equal. Consequently the normalized [linear configuration count](../../../../../linear-configuration-count.md) is

$$
T=\mathbb E_{x,y}f(x)f(y)f(-x-y)=\frac{|A|}{N^2}=\frac\alpha N.
$$

Set $\omega=e^{2\pi i/3}$ and use [Fourier analysis on a finite abelian group](../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) with

$$
\widehat f(\xi)=\mathbb E_x f(x)\omega^{-\xi\cdot x}.
$$

The [orthogonality of roots of unity](../../../../../orthogonality-of-roots-of-unity.md) and the [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) give

$$
T=\sum_{\xi\in V}\widehat f(\xi)^3,
\qquad
\widehat f(0)=\alpha,
\qquad
\sum_{\xi\ne0}|\widehat f(\xi)|^2=\alpha-\alpha^2.
$$

If $N\alpha^2\geq2$, then $\alpha<1$ for a [cap set](../../../../../cap-set.md) and

$$
\frac{\alpha^3}{2}
\leq\alpha^3-\frac\alpha N
\leq\sum_{\xi\ne0}|\widehat f(\xi)|^3
\leq\left(\max_{\xi\ne0}|\widehat f(\xi)|\right)(\alpha-\alpha^2).
$$

Thus some nonzero [finite abelian Fourier coefficient](../../../../../fourier-coefficient-on-a-finite-abelian-group.md) has magnitude at least $\alpha^2/2$.

For this $\xi$, let $\alpha_j$ be the [subset density](../../../../../density-of-a-finite-subset.md) of $A$ on the [affine subspace](../../../../../affine-subspace.md) $\{x:\xi\cdot x=j\}$, for $j=0,1,2$. These three [affine subspaces](../../../../../affine-subspace.md) have equal [cardinality](../../../../../cardinality.md), and

$$
\alpha=\frac{\alpha_0+\alpha_1+\alpha_2}{3},
\qquad
\widehat f(\xi)=\frac13\sum_{j=0}^2\alpha_j\omega^{-j},
\qquad
\alpha_j-\alpha=2\operatorname{Re}\bigl(\widehat f(\xi)\omega^j\bigr).
$$

Among three directions separated by $2\pi/3$, one makes an angle at most $\pi/3$ with any given complex number. Hence $\max_j(\alpha_j-\alpha)\geq|\widehat f(\xi)|$. Restricting to that [hyperplane](../../../../../hyperplane.md) gives the [hyperplane density increment for cap sets](../../../../../hyperplane-density-increment-for-cap-sets.md)

$$
\alpha'\geq\alpha+\frac{\alpha^2}{2},\qquad d'=d-1.
$$

Translate the [affine subspace](../../../../../affine-subspace.md) to its underlying [vector space](../../../../../vector-space-split.md). This preserves the [cap set](../../../../../cap-set.md) property: translating a triple by $t$ changes its sum by $3t=0$. The same argument can therefore be iterated.

For completeness, the [density increment](../../../../../density-increment.md) iteration gives an explicit uniform bound. If $n<16$, the hypothesis $\alpha\geq16/n$ is impossible. Suppose $n\geq16$ and a [cap set](../../../../../cap-set.md) has $\alpha_0\geq16/n$. For every integer $0\leq t\leq\lfloor n/2\rfloor$, its remaining [dimension](../../../../../dimension-vector-space.md) is at least $n/2$, and its current [subset density](../../../../../density-of-a-finite-subset.md) is at least $16/n$. Thus

$$
3^{n-t}\alpha_t^2\geq3^{n/2}\frac{256}{n^2}\geq2.
$$

The last inequality holds at $n=16$ and remains true as $n$ increases: the successive ratio of $3^{n/2}/n^2$ is $\sqrt3\,(n/(n+1))^2>1$ for $n\geq16$. At each step, as long as the [subset density](../../../../../density-of-a-finite-subset.md) remains at most one,

$$
\frac1{\alpha_t}-\frac1{\alpha_{t+1}}
\geq\frac1{2+\alpha_t}\geq\frac13.
$$

After $L=\lfloor n/2\rfloor$ steps this would imply

$$
0<\frac1{\alpha_L}\leq\frac n{16}-\frac L3<0,
$$

a contradiction. The endpoint $\alpha=1$ already contradicts the [cap set](../../../../../cap-set.md) property in positive [dimension](../../../../../dimension-vector-space.md). This proves the claimed existence of three distinct points and the [Meshulam bound for cap sets](../../../../../meshulam-bound-for-cap-sets.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 111](../../paper-111-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
