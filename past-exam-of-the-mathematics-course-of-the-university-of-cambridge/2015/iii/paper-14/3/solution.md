<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a [standard Borel probability space](../../../../../standard-borel-probability-space.md) so that [conditional measures](../../../../../conditional-measures-of-a-factor.md) can be realized by measures. The [disintegration theorem for a probability measure](../../../../../disintegration-theorem-for-a-probability-measure.md) states the following. For a measurable map $\pi:X\to Y$ between standard Borel spaces and $\nu=\pi_*\mu$, there is a [measurable probability kernel](../../../../../measurable-probability-kernel.md) $y\mapsto\mu_y$, unique for $\nu$-almost every $y$, such that

$$
\boxed{\mu(A)=\int_Y\mu_y(A)\,d\nu(y),\qquad
\mu_y(\pi^{-1}\{y\})=1\quad\text{for }\nu\text{-almost every }y.}
$$

Measurability means $y\mapsto\mu_y(A)$ is measurable for every Borel set $A$. More generally

$$
\int_Xf\,d\mu=\int_Y\left(\int_Xf\,d\mu_y\right)d\nu(y),
\qquad
\mathbb E_\mu[f\mid\pi^{-1}\mathcal B_Y](x)
=\int_Xf\,d\mu_{\pi(x)}
$$

for integrable $f$, with equality of the last expression [almost everywhere](../../../../../almost-everywhere.md). The $\mu_y$ are the [conditional measures of a factor](../../../../../conditional-measures-of-a-factor.md). This also defines [conditional measures](../../../../../conditional-measures-of-a-factor.md) for a countably generated sub-sigma-algebra, or a measurable partition represented by such a map. Sigma-algebras are considered modulo null sets where necessary.

For an invariant [probability measure](../../../../../probability-measure.md), disintegrate over the [invariant sigma-algebra](../../../../../invariant-sigma-algebra.md) $\mathcal I$. On a standard probability space it can be represented, modulo null sets, by a countably generated measurable factor $\pi$. One justification for this countability is the separability of $L^2$: a countable dense family of $\mathcal I$-measurable functions generates $\mathcal I$ modulo null sets. **The resulting [conditional measures](../../../../../conditional-measures-of-a-factor.md) are the [ergodic components](../../../../../ergodic-component.md)**:

$$
\boxed{\mu=\int_Y\mu_y\,d\nu(y),\qquad
\mathbb E_\mu[f\mid\mathcal I](x)=\int f\,d\mu_{\pi(x)}.}
$$

Their invariance is one of the permitted facts. It remains to prove that almost every component is [ergodic](../../../../../ergodicity.md), rather than simply invariant.

Choose a [countable generating algebra](../../../../../countable-generating-algebra.md) $\mathcal A$ generating the Borel sigma-algebra of $X$. Apply the [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) simultaneously to its indicators. For $\mu$-almost every $z$ and all $A\in\mathcal A$,

$$
\frac1N\sum_{n<N}\mathbf1_A(T^nz)
\longrightarrow\mathbb E_\mu[\mathbf1_A\mid\mathcal I](z)
=\mu_{\pi(z)}(A).
$$

Disintegration transfers this common full-measure set to $\mu_y$-almost every $z$, for $\nu$-almost every $y$. On that fiber the [conditional expectation](../../../../../conditional-expectation.md) is constant and equals $\mu_y(A)$. Thus, simultaneously for every $A\in\mathcal A$,

$$
\frac1N\sum_{n<N}\mathbf1_A(T^nz)\longrightarrow\mu_y(A)
\quad\text{for }\mu_y\text{-almost every }z.
$$

Fix such a $y$, for which $\mu_y$ is also invariant. Applying the [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) to the system with measure $\mu_y$ identifies these limits with

$$
\mathbb E_{\mu_y}[\mathbf1_A\mid\mathcal I_y]=\mu_y(A).
$$

Finite linear combinations of the algebra's indicators are dense in $L^2(\mu_y)$, by the [Monotone class theorem](../../../../../monotone-class-theorem.md). Since [conditional expectation](../../../../../conditional-expectation.md) is an $L^2$ contraction, its projection onto invariant functions consequently sends every $L^2(\mu_y)$ function to its constant integral. In particular, for any $\mu_y$-invariant set $D$,

$$
\mathbf1_D=\mathbb E_{\mu_y}[\mathbf1_D\mid\mathcal I_y]
=\mu_y(D)\quad\mu_y\text{-almost everywhere},
$$

and so $\mu_y(D)\in\{0,1\}$. This proves **almost every component is [ergodic](../../../../../ergodicity.md)**. The [countable-test proof of ergodicity of conditional components](../../../../../countable-test-proof-of-ergodicity-of-conditional-components.md) avoids taking an invalid intersection of uncountably many full-measure sets.

For rotation by $1/5$, take the quotient map $\pi(x)=5x\pmod1$. Its fibers are exactly the five-point orbits. The [ergodic components of a rational circle rotation](../../../../../ergodic-components-of-a-rational-circle-rotation.md) are therefore

$$
\boxed{\mu_y=\frac15\sum_{j=0}^4
\delta_{(y+j)/5},\quad y\in[0,1),\qquad
m=\int_0^1\mu_y\,dy.}
$$

Equivalently the component through $x$ is $\frac15\sum_{j=0}^4\delta_{x+j/5}$. To check the disintegration, for bounded measurable $f$ use the change of variables on the five consecutive fifth-intervals:

$$
\int_0^1\frac15\sum_{j=0}^4f\!\left(\frac{y+j}{5}\right)dy
=\sum_{j=0}^4\int_{j/5}^{(j+1)/5}f(x)\,dx
=\int_0^1f(x)\,dx.
$$

The rotation cyclically permutes the five atoms, preserving their equal masses. A set invariant modulo $\mu_y$ must contain all or none of this finite orbit, since every atom has positive mass. Thus each $\mu_y$ is [ergodic](../../../../../ergodicity.md). Finally, the [invariant sigma-algebra](../../../../../invariant-sigma-algebra.md) is the pullback under $\pi$: a function invariant under translation by $1/5$ is constant on each orbit and is a measurable function of $5x\pmod1$. This confirms that these are the [conditional measures](../../../../../conditional-measures-of-a-factor.md) over $\mathcal I$, not merely some decomposition into invariant measures.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
