<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Set $z=x^2/\varepsilon$. The differential operator simplifies because its first-[derivative](../../../../../derivative.md) terms cancel:

$$
\varepsilon^2\left(y_{xx}-\frac{y_x}x\right)-4x^2y
=4x^2(y_{zz}-y).
$$

Thus the homogeneous solutions are $e^{\pm z}$ and the transformed forcing is $1/(4\varepsilon z)$. For the decaying-sector [variation of parameters](../../../../../variation-of-parameters.md) solution choose **the contour directions**

$$
\boxed{\theta_1=0,\qquad\theta_2=\pi/2.}
$$

The first integrand decays at positive-real infinity and the second at positive-imaginary infinity. Join each endpoint to $x$ within the first quadrant, avoiding zero. This also fixes the exponentially small homogeneous contributions, which cannot be determined from an algebraic [asymptotic expansion](../../../../../asymptotic-expansion.md) alone.

After $s=t^2/\varepsilon$, write $A(z)=\int_{+\infty}^z e^{-s}\,ds/s$ and $B(z)=\int_{-\infty+i0}^z e^s\,ds/s$. Their [derivatives](../../../../../derivative.md) are $A'=e^{-z}/z$ and $B'=e^z/z$. Direct differentiation of $y=(e^zA-e^{-z}B)/(8\varepsilon)$ gives $y_{zz}-y=1/(4\varepsilon z)$, verifying the original equation. In terms of the [exponential integral](../../../../../exponential-integral.md), with the logarithm continued through the upper half-plane,

$$
\boxed{y=-\frac1{8\varepsilon}\left[e^zE_1(z)+e^{-z}\bigl(\operatorname{Ei}(z)-i\pi\bigr)\right].}
$$

The $-i\pi$ is essential: the contour for $B$ starts at argument $\pi$, not at real positive infinity. On the positive real axis this choice gives the imaginary part $\pi e^{-z}/(8\varepsilon)$.

Repeated endpoint [integration by parts](../../../../../integration-by-parts.md) gives $e^zE_1(z)\sim z^{-1}(1-z^{-1}+2!z^{-2}-\cdots)$ and the matching expansion of $e^{-z}(\operatorname{Ei}(z)-i\pi)$ with positive factorial coefficients in the upper-half-plane sector. Their odd inverse-power corrections cancel. Therefore **the leading large-$x$ term in the requested quadrant is**

$$
\boxed{y(x)\sim-\frac1{4x^2}.}
$$

Use the convention that [anti-Stokes lines](../../../../../anti-stokes-line.md) have equal exponential magnitudes, $\operatorname{Re}(x^2/\varepsilon)=0$. They are $\arg x=\pi/4+m\pi/2$. The [Stokes lines](../../../../../stokes-line.md) are $\arg x=m\pi/2$. Continuing this same solution below the positive-real ray switches on $i\pi e^{-z}/(4\varepsilon)$; continuing above the positive-imaginary ray switches on $i\pi e^z/(4\varepsilon)$. These exponentials remain decaying up to the neighbouring [anti-Stokes lines](../../../../../anti-stokes-line.md). Hence **the maximal adjacent decay sector on this continuation is**

$$
\boxed{-\pi/4<\arg x<3\pi/4.}
$$

On its two boundary rays the switched exponential has constant modulus and oscillates, so $y$ does not tend to zero. Within the sector the leading algebraic term above persists. The internal [anti-Stokes line](../../../../../anti-stokes-line.md) at $\pi/4$ presents no growing exponential for the chosen solution.

For the formal small-$\varepsilon$ series, substitution and comparison of successive powers gives $a_0=1$ and $a_r=2r(2r-1)a_{r-1}$. Thus **all coefficients are**

$$
\boxed{a_r=(2r)!,\qquad
y\sim-\frac1{4\varepsilon}\sum_{r\geq0}\frac{(2r)!}{z^{2r+1}}.}
$$

This is a factorially divergent [asymptotic expansion](../../../../../asymptotic-expansion.md). The ratio of consecutive term magnitudes is $(2r+2)(2r+1)/|z|^2$. For [optimal truncation](../../../../../optimal-truncation.md), retain $r=0,\ldots,n-1$, choosing $2n=|z|+O(1)$, so the cutoff is at a least term.

To resolve the remainder near the positive-real [Stokes line](../../../../../stokes-line.md), use its exact [Borel integral with a simple pole](../../../../../borel-integral-with-a-simple-pole.md):

$$
y=-\frac1{4\varepsilon}\int_{\mathcal C_-}\frac{e^{-zt}}{1-t^2}\,dt,
\qquad
R_n=-\frac{e^{-z}}{4\varepsilon}\int_{\mathcal C_-}\frac{t^{2n}e^{z(1-t)}}{1-t^2}\,dt.
$$

Here $\mathcal C_-$ runs from zero to positive-real infinity below the pole at one. Partial fractions reproduce the exponential-integral solution, including its positive imaginary part. The finite geometric identity for $(1-t^2)^{-1}$ gives the displayed exact remainder after integrating the first $n$ monomials.

Write $z=2n+i\mu\sqrt n+\nu$, with real bounded $\mu$ and bounded $\nu$. For a [Gaussian saddle coalescing with a simple pole](../../../../../gaussian-saddle-coalescing-with-a-simple-pole.md), put $t=1+u/\sqrt n$. The exponent becomes $-u^2-i\mu u+O(n^{-1/2})$ and $dt/(1-t^2)=-du/(2u)+O(n^{-1/2})\,du$. Therefore

$$
J_n\sim-\frac12\int_{\mathcal C_-}\frac{e^{-u^2-i\mu u}}u\,du.
$$

The integral is its [Cauchy principal value](../../../../../cauchy-principal-value.md) plus $i\pi$. If $F(\mu)=\operatorname{PV}\int_{\mathbb R}e^{-u^2-i\mu u}\,du/u$, differentiation gives $F'(\mu)=-i\sqrt\pi e^{-\mu^2/4}$ and $F(0)=0$. Consequently $F(\mu)=-i\pi\operatorname{erf}(\mu/2)$, and $J_n=-i\pi\operatorname{erfc}(\mu/2)/2+O(n^{-1/2})$.

For $x=\rho e^{i\theta}$ with fixed $\rho>0$ and $\theta=O(\sqrt\varepsilon)$, $\mu/2=\sqrt2\rho\theta/\sqrt\varepsilon+O(\varepsilon)$. The [error-function smoothing of a Stokes multiplier](../../../../../error-function-smoothing-of-a-stokes-multiplier.md) therefore gives **the optimally truncated remainder**

$$
\boxed{R_n=\frac{i\pi}{8\varepsilon}e^{-x^2/\varepsilon}
\operatorname{erfc}\!\left(\frac{\sqrt2\rho\theta}{\sqrt\varepsilon}\right)
+O\!\left(\frac{|e^{-x^2/\varepsilon}|}{\varepsilon\sqrt{|z|}}\right).}
$$

The error estimate is uniform for bounded $\theta/\sqrt\varepsilon$. On the [Stokes line](../../../../../stokes-line.md) the multiplier is half its switched-on value; above it the exponentially small term switches off, and below it switches on. This term is invisible at every algebraic order. Near the line the remainder can exceed the least retained term by a square-root factor because a pole meets the [saddle point](../../../../../saddle-point.md).

The printed auxiliary Gaussian hint has inconsistent constants. Direct [saddle point](../../../../../saddle-point.md) expansion of its nonsingular integral gives $\frac12\sqrt{\pi/n}\,e^{-\mu^2/4}$ under its printed scaling, rather than $\frac12\sqrt{\pi/(2n)}\,e^{-\mu^2/8}$. The derivation above uses the correct [saddle point](../../../../../saddle-point.md) normalization and independently fixes both the smoothing width and the contour sign.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
