# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_203.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded, relatively closed set $A\subset\mathbb H$ for which $\mathbb H\setminus A$ is [simply connected domain](../../../complex-analysis.md#simply-connected-domain). Its [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the unique [conformal map](../../../geometry-and-topology.md#conformal-map) $g_A:\mathbb H\setminus A\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity)

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

The [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is

$$
\boxed{\operatorname{hcap}(A)=a.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Let $g=g_A$ and define $u(z)=\operatorname{Im}(z-g(z))$. This is [harmonic](../../../partial-differential-equation.md#harmonic-function) on $\mathbb H\setminus A$, has boundary values $\operatorname{Im}z$ on the hull boundary and zero on the real boundary, and tends to zero at infinity. The representation by [harmonic measure](../../../brownian-motion.md#harmonic-measure) and [optional sampling theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) therefore give

$$
u(z)=\mathbb E_z[\operatorname{Im}B_\tau].
$$

At $z=iy$, the hydrodynamic expansion gives

$$
u(iy)=\operatorname{Im}\left(-\frac{a}{iy}+O(y^{-2})\right)
=\frac{a}{y}+O(y^{-2}).
$$

Consequently the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) is

$$
\boxed{\operatorname{hcap}(A)=
\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau].}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Map out $A$ first. The image

$$
D=g_A(C\setminus A)
$$

with its bounded filling is a [compact H-hull](../../../stochastic-process.md#compact-h-hull), and uniqueness of hydrodynamic normalization gives

$$
g_C=g_D\circ g_A.
$$

Comparing the coefficients of $1/z$ at infinity yields the [half-plane-capacity composition rule](../../../stochastic-process.md#half-plane-capacity-composition-rule)

$$
\operatorname{hcap}(C)
=\operatorname{hcap}(A)+\operatorname{hcap}(D)
\geq\operatorname{hcap}(A).
$$

Thus **half-plane capacity is monotone under inclusion**.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The statement is **true**. In the notation of part (ii), equality of the capacities forces $\operatorname{hcap}(D)=0$. Every nonempty [compact H-hull](../../../stochastic-process.md#compact-h-hull) has strictly positive half-plane capacity: by the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity), Brownian motion started sufficiently high has positive harmonic measure of a boundary portion of positive height. Hence $D=\varnothing$, so $C\setminus A=\varnothing$ and

$$
\boxed{A=C.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The family is a [nondecreasing family of sets](../../../set.md#nondecreasing-family-of-sets) when

$$
A_s\subseteq A_t\qquad(0\leq s\leq t).
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

It has the [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) under the standard chordal convention when

$$
\boxed{\operatorname{hcap}(A_t)=2t.}
$$

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

It has the [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) when, after mapping out the old hull, each short new increment is small: for every $T,\epsilon>0$ there is $\delta>0$ such that

$$
0\leq s<t\leq T,\quad t-s<\delta
\quad\Longrightarrow\quad
\operatorname{diam}\bigl(g_s(A_t\setminus A_s)\bigr)<\epsilon.
$$

Equivalent formulations use a crosscut of diameter below $\epsilon$ separating the new increment from infinity.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $r_t=\sqrt{2t}$. The hulls $A_t=r_t(\mathbb H\cap\mathbb D)$ are nested, so property (i) holds. Scaling the given map gives

$$
g_t(z)=z+\frac{r_t^2}{z}=z+\frac{2t}{z},
$$

so $\operatorname{hcap}(A_t)=2t$ and property (ii) holds.

Property (iii) fails. For $s>0$, the image under $g_s$ of the outer semicircle of $A_t\setminus A_s$ is

$$
g_s(r_te^{i\theta})
=r_te^{i\theta}+\frac{r_s^2}{r_te^{i\theta}}.
$$

As $t\downarrow s$, this converges to $2r_s\cos\theta$, which fills the real interval $[-2r_s,2r_s]$. Hence the diameter of the mapped new increment tends to $4r_s$, rather than zero. Therefore **(i) and (ii) hold, while (iii) does not**.

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

If $g_t$ is driven by $U_t=\sqrt\kappa B_t$, then the mapping-out functions of

$$
\widetilde\gamma(t)=r\gamma(t/r^2)
$$

are

$$
\widetilde g_t(z)=r g_{t/r^2}(z/r),
$$

and their driver is $\widetilde U_t=rU_{t/r^2}$. By [Brownian scaling](../../../brownian-motion.md#brownian-scaling), $(rB_{t/r^2})_{t\geq0}$ is Brownian. Thus $\widetilde U$ has the same law as $U$, and uniqueness of the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) proves

$$
\boxed{(r\gamma(t/r^2))_{t\geq0}\overset d=(\gamma(t))_{t\geq0}.}
$$

This is the [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $D$ be [simply connected domain](../../../complex-analysis.md#simply-connected-domain) with distinct marked boundary points $a,b$, and choose a [conformal map](../../../geometry-and-topology.md#conformal-map) $f:D\to\mathbb H$ with $f(a)=0$ and $f(b)=\infty$. Chordal $\operatorname{SLE}_\kappa$ from $a$ to $b$ is the unparameterized curve $f^{-1}(\gamma)$, where $\gamma$ is chordal SLE in $(\mathbb H,0,\infty)$.

Any other such map is $\widetilde f=rf$ for some $r>0$. The [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) says that $r^{-1}\gamma$ has the same unparameterized law as $\gamma$; only its capacity clock changes. Hence the pullback law is independent of $f$. This proves the [Conformal invariance of SLE](../../../stochastic-process.md#conformal-invariance-of-sle) definition is well-defined.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Put

$$
p=\frac{8-\kappa}{8}>0,
\qquad q=\frac{8-\kappa}{\kappa}>0,
$$

so $M_t=\Upsilon_t^{-p}S_t^q$. Before $\tau_\epsilon$, one has $\Upsilon_t\geq\epsilon$ and $0<S_t\leq1$. Therefore

$$
0\leq M_{t\wedge\tau_\epsilon}\leq\epsilon^{-p}.
$$

The supplied continuous local martingale is thus bounded after stopping, and a bounded local martingale is a true martingale. Hence

$$
\boxed{(M_{t\wedge\tau_\epsilon})_{t\geq0}
\text{ is a bounded martingale}.}
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

At time zero, $\Upsilon_0(z)=\operatorname{Im}z$. Compactness of $K\subset\mathbb H$ gives

$$
\epsilon_0=\min_{z\in K}\operatorname{Im}z>0.
$$

Also $M_0(z)$ is uniformly bounded above on $K$. On

$$
E_\epsilon=\{\tau_\epsilon<\infty, S_{\tau_\epsilon}\geq1/2\},
$$

one has $M_{\tau_\epsilon}\geq\epsilon^{-p}2^{-q}$. Optional stopping, [Fatou lemma](../../../measure-theory.md#fatou-s-lemma), and the assumed conditional angular estimate give

$$
\sup_{z\in K}M_0(z)
\geq\mathbb E[M_{\tau_\epsilon};E_\epsilon]
\geq\epsilon^{-p}2^{-q}c_1
\mathbb P(\tau_\epsilon<\infty).
$$

Thus

$$
\boxed{\mathbb P_z(\tau_\epsilon<\infty)
\leq C_K\epsilon^{(8-\kappa)/8}.}
$$

The exponent $(8-\kappa)/\kappa$ requested in the question does not follow and is false as written. The [SLE Green-function estimate](../../../stochastic-process.md#sle-green-function-estimate) gives probability comparable to $\epsilon^{1-\kappa/8}$, confirming that the denominator in the requested exponent should be $8$.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

For compact $K\subset\mathbb H$, let

$$
E_\epsilon=\{z\in K:\tau_\epsilon(z)<\infty\}.
$$

By the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) and part (ii),

$$
\mathbb E[\operatorname{Leb}(E_\epsilon)]
=\int_K\mathbb P_z(\tau_\epsilon<\infty)\,dz
\leq C_K\operatorname{Leb}(K)\epsilon^{(8-\kappa)/8}
\longrightarrow0.
$$

Every point in the SLE range has conformal radius tending to zero and therefore belongs to every $E_\epsilon$. Hence the range inside $K$ has zero expected [Lebesgue measure](../../../measure-theory.md#lebesgue-measure), and so has zero measure almost surely. Exhausting $\mathbb H$ by countably many compact sets proves

$$
\boxed{\operatorname{Leb}(\gamma[0,\infty))=0\quad\text{almost surely}.}
$$

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace) is

$$
\boxed{
\begin{array}{c|c}
0\leq\kappa\leq4&\text{simple}\\
4<\kappa<8&\text{self-intersecting but not space-filling}\\
\kappa\geq8&\text{space-filling}.
\end{array}}
$$

At $\kappa=0$ the trace is the deterministic vertical slit.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a real boundary point $x\ne0$, set

$$
X_t=\frac{g_t(x)-U_t}{\sqrt\kappa}.
$$

After a deterministic rescaling of time, the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) says that $X$ is a [Bessel process](../../../brownian-motion.md#bessel-process) of dimension

$$
\delta=1+\frac4\kappa.
$$

When $0<\kappa\leq4$, one has $\delta\geq2$, and the [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process) says that $X$ never reaches zero. Thus no nonzero real boundary point is swallowed. The standard Loewner trace criterion then implies that each new tip is attached only to the preceding tip and the trace never intersects its past, so it is simple. For $\kappa=0$, the equation is driven by zero and generates a vertical slit. Hence **$\operatorname{SLE}_\kappa$ is simple for $0\leq\kappa\leq4$**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Let $Z_t=g_t(z)-U_t$. For $\operatorname{SLE}_4$, $dU_t=2dB_t$, and the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives

$$
dZ_t=\frac2{Z_t}dt-2dB_t,
\qquad d\langle Z\rangle_t=4dt.
$$

The complex [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) yields

$$
d\log Z_t
=\frac1{Z_t}dZ_t-\frac1{2Z_t^2}d\langle Z\rangle_t
=-\frac2{Z_t}dB_t.
$$

Therefore

$$
\boxed{\log(g_t(z)-U_t)\text{ is a continuous local martingale}.}
$$

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The imaginary part

$$
\arg(g_t(z)-U_t)
$$

is a bounded local martingale and hence a martingale. As the simple transient trace passes $z$, this angle converges to $\pi$ if the trace passes to the right of $z$ and to $0$ if it passes to the left. Bounded convergence therefore gives

$$
\arg z
=\pi\,\mathbb P(\gamma\text{ passes to the right of }z),
$$

so the [SLE4 left-passage probability](../../../stochastic-process.md#sle4-left-passage-probability) is

$$
\boxed{\mathbb P(\gamma\text{ passes to the right of }z)
=\frac{\arg z}{\pi}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Fix $z$ and write

$$
L_t(z)=\log(g_t(z)-U_t).
$$

By assumption, $L(z)$ is a continuous local martingale, so $Z_t(z)=e^{L_t(z)}$ is a [semimartingale](../../../stochastic-calculus.md#semimartingale). The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives

$$
g_t(z)=z+\int_0^t\frac2{Z_s(z)}ds,
$$

which has [finite variation](../../../real-analysis.md#total-variation-of-a-function). Therefore

$$
U_t=g_t(z)-Z_t(z)
$$

is a semimartingale. Thus **the Loewner driver $U$ is a continuous semimartingale**.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

Write the [semimartingale decomposition](../../../stochastic-calculus.md#semimartingale-decomposition) as $U=M+A$, where $M$ is a continuous local martingale and $A$ has finite variation. Applying [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\log Z_t(z)$ shows that its finite-variation part is

$$
\frac{2}{Z_t(z)^2}dt
-\frac1{Z_t(z)}dA_t
-\frac1{2Z_t(z)^2}d\langle M\rangle_t.
$$

It vanishes for every $z$. Multiplying by $Z_t(z)^2$ gives

$$
2dt-Z_t(z)dA_t-\frac12d\langle M\rangle_t=0.
$$

Subtract this identity for two points with distinct $Z_t$ to obtain $dA_t=0$; then $d\langle M\rangle_t=4dt$. Since the curve starts at zero, $U_0=0$. The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) now gives $U_t=2B_t$. Hence the Loewner chain is

$$
\boxed{\operatorname{SLE}_4.}
$$

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The law satisfies the [chordal restriction property](../../../stochastic-process.md#chordal-restriction-property) when, for every $A\in\mathcal Q_\pm$, conditional on $\gamma\cap A=\varnothing$, the mapped curve $\psi_A(\gamma)$ has the same unparameterized law as $\gamma$ in $(\mathbb H,0,\infty)$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Assume the avoidance formula. Given another admissible hull $C$, put $D=A\cup\psi_A^{-1}(C)$ with the bounded filling. Uniqueness of the normalized maps gives

$$
\psi_D=\psi_C\circ\psi_A,
\qquad
\psi_D'(0)=\psi_C'(0)\psi_A'(0).
$$

Therefore

$$
\begin{aligned}
\mathbb P(\psi_A(\gamma)\cap C=\varnothing\mid\gamma\cap A=\varnothing)
&=\frac{\mathbb P(\gamma\cap D=\varnothing)}
{\mathbb P(\gamma\cap A=\varnothing)}\\
&=\frac{\psi_D'(0)^\alpha}{\psi_A'(0)^\alpha}
=\psi_C'(0)^\alpha.
\end{aligned}
$$

These avoidance events determine the law of a simple closed random set. They agree with those of $\gamma$, so the conditional mapped law equals the original law. Hence the avoidance formula implies the [chordal restriction property](../../../stochastic-process.md#chordal-restriction-property).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $J_t=\psi_t'(U_t)$, $q_t=\psi_t''(U_t)/\psi_t'(U_t)$, and $r_t=(\partial_z^3\psi_t)(U_t)/\psi_t'(U_t)$. Since $dU_t=\sqrt{8/3}\,dB_t$, the supplied identity and [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) give

$$
d\log J_t
=q_t\,dU_t
+\left[-\frac56q_t^2
+\left(-\frac43+\frac12\frac83\right)r_t\right]dt
=q_t\,dU_t-\frac56q_t^2dt.
$$

For $M_t=J_t^\alpha$, its drift coefficient is

$$
-\frac{5\alpha}{6}+\frac12\alpha^2\frac83
=\frac{\alpha(8\alpha-5)}6.
$$

Thus the nonzero choice is

$$
\boxed{\alpha=\frac58,}
$$

and $M_{t\wedge\tau}$ is a continuous local martingale. The boundary Schwarz lemma for mapping-out maps gives $0\leq J_{t\wedge\tau}\leq1$, so $0\leq M_{t\wedge\tau}\leq1$. A bounded local martingale is a true martingale. This is the [SLE eight-thirds restriction martingale](../../../stochastic-process.md#sle-eight-thirds-restriction-martingale).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

Let $A=\mathbb H\cap B(1,\epsilon)$. Its normalized mapping-out map is

$$
\psi_A(z)=z+\frac{\epsilon^2}{z-1}+\epsilon^2,
$$

so $\psi_A(0)=0$ and

$$
\psi_A'(0)=1-\epsilon^2.
$$

Using the restriction exponent $5/8$ gives

$$
\boxed{\mathbb P\bigl(\gamma[0,\infty)\cap
(\mathbb H\cap B(1,\epsilon))=\varnothing\bigr)
=(1-\epsilon^2)^{5/8}.}
$$

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

For the vertical slit $A=(1,1+i\epsilon]$, choose the square-root branch asymptotic to $z-1$ at infinity. The normalized map is

$$
\psi_A(z)=\sqrt{(z-1)^2+\epsilon^2}+\sqrt{1+\epsilon^2},
$$

for which $\psi_A(0)=0$ and

$$
\psi_A'(0)=\frac1{\sqrt{1+\epsilon^2}}.
$$

Therefore

$$
\boxed{\mathbb P\bigl(\gamma[0,\infty)\cap(1,1+i\epsilon]
=\varnothing\bigr)
=(1+\epsilon^2)^{-5/16}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
