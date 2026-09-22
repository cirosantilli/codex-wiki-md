<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use Planck units and restrict to the physical [Kähler metric](../../../../../kahler-metric.md) domain

$$
x=S+\bar S>0,\qquad y=T+\bar T-|C|^2>0.
$$

Put $A=ae^{-\alpha S}$ and $w=A+b$, so that $W=C^3+w$. There are no gauged interactions specified, hence no additional [D-term scalar potential](../../../../../d-term-scalar-potential.md). The [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) is $V=e^K(K^{i\bar j}D_iW\overline{D_jW}-3|W|^2)$, with $e^K=1/(xy^3)$. Its [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) are

$$
D_SW=-\alpha A-\frac W x,\qquad D_TW=-\frac{3W}{y},\qquad D_CW=3C^2+\frac{3\bar C W}{y}.
$$

The nonzero metric entries are

$$
K_{S\bar S}=x^{-2},\quad
\begin{pmatrix}K_{T\bar T}&K_{T\bar C}\\K_{C\bar T}&K_{C\bar C}\end{pmatrix}
=\frac3{y^2}\begin{pmatrix}1&-C\\-\bar C&T+\bar T\end{pmatrix}.
$$

The determinant of this $T,C$ block is $9/y^3>0$, so it is positive definite. With the inverse-index convention $K_{i\bar j}K^{k\bar j}=\delta_i^k$, the raised components are

$$
K^{S\bar S}=x^2,\qquad
\begin{pmatrix}K^{T\bar T}&K^{T\bar C}\\K^{C\bar T}&K^{C\bar C}\end{pmatrix}
=\frac y3\begin{pmatrix}T+\bar T&\bar C\\C&1\end{pmatrix}.
$$

Keeping these complex-conjugate off-diagonal entries in their correct index positions is essential.

To exhibit the [no-scale supergravity](../../../../../no-scale-supergravity.md) cancellation, write the $T,C$ norm as

$$
K^{i\bar j}D_iW\overline{D_jW}\big|_{T,C}
=\frac y3\left[y|D_TW|^2+|D_CW+\bar C D_TW|^2\right]
=3|W|^2+3y|C|^4.
$$

Here $D_CW+\bar C D_TW=3C^2$. The $3|W|^2$ term cancels the negative term in the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md). The result is **the nonnegative scalar potential**

$$
\boxed{V=\frac{|C^3+b+(1+\alpha x)A|^2}{xy^3}+\frac{3|C|^4}{xy^2}.}
$$

This is the [matter-logarithm no-scale potential](../../../../../matter-logarithm-no-scale-potential.md), specialized to the exponential [superpotential](../../../../../superpotential.md).

Choose the [supergravity auxiliary field](../../../../../supergravity-auxiliary-field.md) convention $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$. Substitution into the full inverse [Kähler metric](../../../../../kahler-metric.md) gives

$$
\boxed{\begin{aligned}
F^S&=e^{K/2}x\,\overline{C^3+b+(1+\alpha x)A},\\
F^T&=e^{K/2}y\,\overline{A+b},\\
F^C&=-e^{K/2}y\,\bar C^2.
\end{aligned}}
$$

An overall auxiliary-field phase is conventional. The $C$ dependence of $F^T$ cancels between the two metric terms. If all three [auxiliary fields](../../../../../auxiliary-field.md) vanished at a finite physical point, $F^C=0$ would force $C=0$, $F^T=0$ would force $A+b=0$, and $F^S=0$ would then force $\alpha x A=0$. Thus $a=b=0$ is necessary. **For any nontrivial choice of $a,b$, supersymmetry is broken at every finite physical point.** The allowed exception $a=b=0$, $C=0$ is supersymmetric; the statement cannot hold for all arbitrary parameters without this qualification.

The [no-scale volume runaway criterion](../../../../../no-scale-volume-runaway-criterion.md) also determines whether the minimum is attained. For fixed $S,C$, differentiation with respect to $y$ gives

$$
\frac{\partial V}{\partial y}=-\frac{3|C^3+b+(1+\alpha x)A|^2}{xy^4}-\frac{6|C|^4}{xy^3}.
$$

It is negative unless both numerators vanish. Therefore a finite stationary vacuum must satisfy

$$
\boxed{C=0,\qquad b+(1+\alpha x)ae^{-\alpha S}=0.}
$$

Every such point is a global minimum with **$V_{\min}=0$**. For $a,b\ne0$, setting $r=|b/a|$ and $z=\alpha x>0$ reduces existence to

$$
r=(1+z)e^{-z/2},\qquad \arg a-\alpha\operatorname{Im}S=\arg(-b)\pmod{2\pi}.
$$

The derivative of the magnitude function is $(1-z)e^{-z/2}/2$. It rises from $1$ at the excluded boundary $z=0$ to $2e^{-1/2}$ at $z=1$, then falls to zero. Consequently **a finite zero-energy minimum exists exactly when**

$$
\boxed{a,b\ne0,\quad 0<|b/a|\le2e^{-1/2},}
$$

or in the separate trivial family $a=b=0$. There is one positive root for $0<r\le1$, two for $1<r<2e^{-1/2}$, and one double root at equality. If only one of $a,b$ vanishes, or $r$ exceeds this maximum, there is no finite minimum: the infimum is zero as $\operatorname{Re}T\to\infty$. Calling this runaway a finite zero-energy vacuum would be incorrect.

At a nontrivial zero-energy minimum, $W=A+b=-\alpha x A\ne0$, and the auxiliary expectation values reduce to

$$
F^S=F^C=0,\qquad F^T=e^{K/2}y\bar W\ne0.
$$

This explicitly verifies [supersymmetry breaking](../../../../../supersymmetry-breaking.md) with zero [vacuum energy](../../../../../vacuum-energy.md) in [no-scale supergravity](../../../../../no-scale-supergravity.md). Both real components of $T$ are exact [flat directions of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md) on the minimum locus. Away from that locus, $\operatorname{Im}T$ is still absent from the potential, but $\operatorname{Re}T$ is not flat. At a minimum, $C$ is lifted at quartic order: at fixed $S,T$, $V=3|C|^4/[x(T+\bar T)^2]+O(|C|^6)$. A zero quadratic mass does not make $C$ an exact flat direction. The [quartic stabilization at a double no-scale root](../../../../../quartic-stabilization-at-a-double-no-scale-root.md) likewise gives a vanishing quadratic mass, but no exact flat direction, for $\operatorname{Re}S$ at $z=1$. For $a=b=0$, the whole $C=0$ family has both $S$ and $T$ flat and [supersymmetry](../../../../../supersymmetry-split.md) unbroken.

Finally, the [gravitino mass from a superpotential](../../../../../gravitino-mass-from-a-superpotential.md) is

$$
\boxed{m_{3/2}=\frac{|C^3+A+b|}{\sqrt{x}\,y^{3/2}}.}
$$

At a nontrivial zero-energy minimum this becomes

$$
\boxed{m_{3/2}=\frac{\alpha\sqrt{x}|A|}{y^{3/2}}=\frac{\alpha\sqrt{x}|b|}{(1+\alpha x)y^{3/2}}>0.}
$$

It depends on the unfixed volume modulus, so the model does not predict one numerical mass. For $a=b=0$, $C=0$, the [gravitino](../../../../../gravitino.md) is massless.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
