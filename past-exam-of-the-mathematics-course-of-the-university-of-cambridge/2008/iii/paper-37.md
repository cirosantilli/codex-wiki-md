# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper37.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The initial-value convention is essential. A [continuous finite-variation local martingale is constant](../../../martingale.md#continuous-finite-variation-local-martingale-is-constant), so the conclusion is $M_t=M_0$ up to [indistinguishability of stochastic processes](../../../stochastic-process.md#indistinguishability-of-stochastic-processes). The stated zero conclusion uses the usual zero-start convention $M_0=0$; without it, $M_t\equiv1$ is a counterexample.

Put $N=M-M_0$. Let $V_t$ be its [total-variation process](../../../stochastic-calculus.md#total-variation-process), and stop when either $|N|$ or $V$ reaches $n$. The resulting process $N^{\tau_n}$ is a bounded [continuous local martingale](../../../martingale.md#continuous-local-martingale), hence a true [martingale](../../../martingale.md), and its total variation on every time interval is bounded by $n$. Fix $t$ and take deterministic partitions $0=t_0<\cdots<t_k=t$ whose mesh tends to zero. Orthogonality of [martingale](../../../martingale.md) increments gives

$$
\mathbb E(N^{\tau_n}_t)^2=\sum_{j=1}^k\mathbb E\bigl(N^{\tau_n}_{t_j}-N^{\tau_n}_{t_{j-1}}\bigr)^2.
$$

Pathwise,

$$
\sum_j\bigl(N^{\tau_n}_{t_j}-N^{\tau_n}_{t_{j-1}}\bigr)^2
\leq\max_j|N^{\tau_n}_{t_j}-N^{\tau_n}_{t_{j-1}}|\,V_t(N^{\tau_n})\longrightarrow0
$$

by uniform continuity of a continuous path on $[0,t]$. The sums are bounded by $2n^2$, so the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) makes their expectations tend to zero. Hence $N^{\tau_n}_t=0$ almost surely. Take the countable intersection over rational $t$ and integer $n$, use path continuity, and then let $n\to\infty$. The [stopping times](../../../martingale.md#stopping-time) tend to infinity because the original path and its [finite variation](../../../real-analysis.md#total-variation-of-a-function) are bounded on every compact time interval. Thus

$$
\boxed{M_t=M_0\text{ for all }t\geq0\text{ outside one null event};\quad M_0=0\Longrightarrow M\equiv0.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

As with [quadratic variation](../../../stochastic-calculus.md#quadratic-variation), the increasing process must be normalized by $A_0=0$. Suppose $A,A'$ have this initial value and both $M^2-A$ and $M^2-A'$ are [continuous local martingales](../../../martingale.md#continuous-local-martingale). Since $M^2$ and these differences are continuous, both $A$ and $A'$ are continuous. Their difference is a [finite-variation process](../../../stochastic-calculus.md#finite-variation-process), and

$$
A-A'=(M^2-A')-(M^2-A)
$$

is a [continuous local martingale](../../../martingale.md#continuous-local-martingale). The result proved in part (a) makes this difference constant. Its initial value is zero, so **$A$ and $A'$ are indistinguishable**. This is the [uniqueness of an increasing square compensator](../../../stochastic-calculus.md#uniqueness-of-an-increasing-square-compensator); it uses no existence argument.

If no initial-value normalization is imposed, the literal uniqueness assertion is false: whenever $A$ works, $A+c$ works for every deterministic constant $c$, since subtracting a constant preserves the [local martingale](../../../martingale.md#local-martingale) property. The exact unnormalized conclusion is $A_t-A'_t=A_0-A'_0$ for all $t$, up to [indistinguishability of stochastic processes](../../../stochastic-process.md#indistinguishability-of-stochastic-processes).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Work first with $M_0=0$. More generally, the assertion needs $M_0\in L^2$ and then applies to $M-M_0$. Without this assumption, an integrable but non-square-integrable initial random variable kept constant in time has zero [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) but is not bounded in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space).

Choose increasing [stopping times](../../../martingale.md#stopping-time)

$$
\tau_n=\inf\{t:|M_t|\geq n\text{ or }[M]_t\geq n\}.
$$

They tend to infinity almost surely, because the continuous path and its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) are finite on every compact time interval. The stopped process is a bounded [martingale](../../../martingale.md), and $M_{t\wedge\tau_n}^2-[M]_{t\wedge\tau_n}$ is bounded and a [local martingale](../../../martingale.md#local-martingale). Taking expectations gives

$$
\mathbb E M_{t\wedge\tau_n}^2=\mathbb E[M]_{t\wedge\tau_n}.
$$

Suppose $C=\mathbb E[M]_\infty<\infty$. These squared expectations are at most $C$. For each fixed $t$, the stopped values converge almost surely to $M_t$ and are uniformly integrable, since they are uniformly bounded in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). They therefore converge in $L^1$. Passing in the stopped conditional-expectation identity, using contraction of [conditional expectation](../../../measure-theory.md#conditional-expectation) in $L^1$, gives $\mathbb E(M_t\mid\mathcal F_s)=M_s$ for $s\leq t$. Thus $M$ is a true [martingale](../../../martingale.md). The [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) gives $\mathbb E M_t^2\leq C$, uniformly in $t$, so it is an [L2-bounded continuous martingale](../../../martingale.md#l2-bounded-continuous-martingale).

Conversely, suppose $M$ is a true [martingale](../../../martingale.md) with $\sup_t\mathbb E M_t^2\leq C$. For fixed $t$, bounded-time [optional sampling theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives $M_{t\wedge\tau_n}=\mathbb E(M_t\mid\mathcal F_{t\wedge\tau_n})$. Conditional [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) then yields

$$
\mathbb E[M]_{t\wedge\tau_n}=\mathbb E M_{t\wedge\tau_n}^2\leq\mathbb E M_t^2\leq C.
$$

The brackets increase to $[M]_t$. Applying the [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) first in $n$ and then in $t\uparrow\infty$ proves $\mathbb E[M]_\infty\leq C<\infty$.

The exact identities and terminal limits can also be justified. On each fixed horizon $t$, the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) gives

$$
\mathbb E\sup_{s\leq t}|M_s|^2\leq4\mathbb E|M_t|^2<\infty.
$$

This is an integrable dominating variable for $M_{t\wedge\tau_n}^2$, so the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) and increasing convergence of the brackets remove the stopping:

$$
\mathbb E M_t^2=\mathbb E[M]_t.
$$

The [L2 martingale convergence theorem](../../../martingale.md#l2-martingale-convergence-theorem) supplies $M_\infty$ with $M_t\to M_\infty$ almost surely and in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). Consequently the squares converge in $L^1$, while $[M]_t\uparrow[M]_\infty$. We obtain the [integrable terminal bracket criterion](../../../martingale.md#integrable-terminal-bracket-criterion) with the precise terminal identity

$$
\boxed{M\text{ is an }L^2\text{-bounded martingale}\iff\mathbb E[M]_\infty<\infty,\qquad\mathbb E M_\infty^2=\mathbb E[M]_\infty.}
$$

For $M_0\in L^2$ rather than zero, the final identity becomes $\mathbb E M_\infty^2=\mathbb E M_0^2+\mathbb E[M]_\infty$.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $r=\|y\|$ and use the ordinary Euclidean [Laplacian](../../../calculus.md#laplacian) $\sum_i\partial_i^2$, so the generator of standard [Brownian motion](../../../brownian-motion.md) is half that operator. For a radial function $f(r)$, the [Laplacian in polar coordinates](../../../calculus.md#laplacian-in-polar-coordinates) is $f''(r)+(d-1)f'(r)/r$. With $f(r)=r^{2-d}$,

$$
f'(r)=(2-d)r^{1-d},\qquad f''(r)=(2-d)(1-d)r^{-d},\qquad\Delta h=0\quad(r>0).
$$

Thus $h$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) on the punctured space.

We first justify that the singularity is not visited. For $0<\eta<x<R$, stop at $S=\tau_\eta\wedge\tau_R$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) makes $h(B_{t\wedge S})$ a [local martingale](../../../martingale.md#local-martingale), and it is bounded on this annulus, hence a true [martingale](../../../martingale.md). The exit time is finite almost surely: $\mathbb P(S>t)\leq\mathbb P(\|B_t\|<R)\to0$ by the Gaussian transition density. Taking the bounded terminal limit yields

$$
\mathbb P(\tau_\eta<\tau_R)\,\eta^{2-d}\leq h(\bar x)=x^{2-d}.
$$

If the origin were reached before $\tau_R$, every smaller radius would first be reached, so letting $\eta\downarrow0$ shows that event has probability zero. Taking a countable sequence $R\to\infty$ proves $\tau_0=\infty$ almost surely. Localization on increasing annuli now applies the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) globally and gives the [Bessel power local martingale](../../../brownian-motion.md#bessel-power-local-martingale)

$$
h(B_t)=h(\bar x)+\int_0^t\nabla h(B_s)\cdot dB_s.
$$

Stopping this [continuous local martingale](../../../martingale.md#continuous-local-martingale) at any $\tau_a$, including $a=0$, preserves its local-[martingale](../../../martingale.md) property.

For $0<a<x$, the stopped path stays at radius at least $a$, so $0<M_t\leq a^{2-d}$. The [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion) makes it a true [martingale](../../../martingale.md). For $a=x$, Brownian radial oscillations at its starting sphere give $\tau_x=0$ almost surely and the stopped process is constant. Thus the same true-[martingale](../../../martingale.md) conclusion holds for $0<a\leq x$.

For $a=0$, the process is a [strict local martingale](../../../martingale.md#strict-local-martingale). To prove this, write $B_t=\bar x+\sqrt t\,G$ in distribution, with $G$ a standard $d$-dimensional normal vector. For every shift $v$,

$$
\mathbb E\|G+v\|^{2-d}\leq1+(2\pi)^{-d/2}\int_{\|u\|\leq1}\|u\|^{2-d}\,du=:C_d<\infty.
$$

Indeed the integrand outside the unit ball is at most one, while inside it the Gaussian density is at most $(2\pi)^{-d/2}$ and the radial integral is a constant times $\int_0^1r\,dr$. [Brownian scaling](../../../brownian-motion.md#brownian-scaling) therefore gives

$$
\mathbb E h(B_t)\leq C_dt^{-(d-2)/2}\longrightarrow0.
$$

A true [martingale](../../../martingale.md) would have expectation $h(\bar x)>0$ at every time, which is impossible.

The printed range also permits $a>x$, and this case must not be grouped with the bounded case. Here $\tau_a<\infty$ almost surely, by the same Gaussian bound for exit from a bounded ball. Moreover,

$$
\mathbb E M_t=a^{2-d}\mathbb P(\tau_a\leq t)+\mathbb E\bigl[h(B_t)\mathbf1_{\{\tau_a>t\}}\bigr]\longrightarrow a^{2-d}<x^{2-d},
$$

since the second expectation is at most $\mathbb E h(B_t)\to0$. It too is a [strict local martingale](../../../martingale.md#strict-local-martingale). The complete [stopped inverse radial power martingale classification](../../../brownian-motion.md#stopped-inverse-radial-power-martingale-classification) is therefore

$$
\boxed{M\text{ is a true martingale for }0<a\leq x;\quad M\text{ is strict local for }a=0\text{ or }a>x.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $0<a<x<b$, put $S=\tau_a\wedge\tau_b$. The process $\phi(\|B_{t\wedge S}\|)$, where $\phi(r)=r^{2-d}$, is a bounded [martingale](../../../martingale.md) by part (a). Also $S<\infty$ almost surely: before exit the endpoint $B_t$ lies inside the radius-$b$ ball, whose Gaussian probability tends to zero as $t\to\infty$. Path continuity makes the terminal radius either $a$ or $b$. If $p=\mathbb P_{\bar x}(\tau_a<\tau_b)$, the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) applied to this bounded stopped [martingale](../../../martingale.md) gives

$$
\phi(x)=p\phi(a)+(1-p)\phi(b).
$$

Solving yields

$$
\boxed{\mathbb P_{\bar x}(\tau_a<\tau_b)=\frac{\phi(b)-\phi(x)}{\phi(b)-\phi(a)}.}
$$

The denominator is nonzero because $\phi$ is strictly decreasing for $d\geq3$.

As $b\uparrow\infty$, the events $\{\tau_a<\tau_b\}$ increase to $\{\tau_a<\infty\}$. In one direction membership already implies a finite hit of $a$; in the other direction a continuous path up to its finite hit of $a$ has a finite maximum radius, so it lies in the event for every sufficiently large $b$. Continuity from below of probability and $\phi(b)\to0$ now give

$$
\boxed{\mathbb P_{\bar x}(\tau_a<\infty)=\frac{x^{2-d}}{a^{2-d}}=\left(\frac ax\right)^{d-2}.}
$$

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Set $N_t=\int_0^tZ_s^{-1}\,dZ_s$, the [stochastic logarithm](../../../stochastic-calculus.md#stochastic-logarithm) of $Z$. On each finite horizon, a strictly positive continuous path has its reciprocal bounded; stopping at levels of $Z$, $Z^{-1}$ and $[Z]$ rigorously localizes this [stochastic integral](../../../stochastic-calculus.md#stochastic-integral). Thus $N$ is a zero-start [continuous local martingale](../../../martingale.md#continuous-local-martingale), with

$$
[N]_t=\int_0^tZ_s^{-2}\,d[Z]_s.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for the ordinary logarithm gives

$$
\log Z_t=\log Z_0+N_t-\frac12[N]_t.
$$

Accordingly, with the exponential convention printed in this question,

$$
\boxed{M_t=\log Z_0+\int_0^t\frac{dZ_s}{Z_s},\qquad Z_t=\exp\!\left(M_t-\frac12[M]_t\right).}
$$

The initial constant in $M$ contributes no [quadratic variation](../../../stochastic-calculus.md#quadratic-variation). Under the standard normalized [Doléans-Dade exponential](../../../stochastic-calculus.md#doleans-dade-exponential) convention, which subtracts the driver's initial value in the exponent, the same formula is written $Z=Z_0\mathcal E(N)$.

For uniqueness, suppose another continuous driver $L$ gives the printed exponential. Evaluating at zero forces $L_0=\log Z_0$. Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to its exponential gives $dZ_t=Z_t\,dL_t$. Since $Z_t>0$, [associativity of stochastic integration](../../../stochastic-calculus.md#associativity-of-stochastic-integration) yields $dL_t=Z_t^{-1}dZ_t$. Thus $L_t=L_0+N_t=M_t$, up to [indistinguishability of stochastic processes](../../../stochastic-process.md#indistinguishability-of-stochastic-processes).

There is an initial-integrability qualification if “[local martingale](../../../martingale.md#local-martingale)” is used with the usual integrable-initial-value definition. The displayed $M$ is a [continuous local martingale](../../../martingale.md#continuous-local-martingale) when $\log Z_0\in L^1$, in particular when $Z_0$ is a positive deterministic number. An arbitrary positive integrable $Z_0$ does not ensure this. For example, take an $\mathcal F_0$-measurable positive integer $W$ with $\mathbb P(W=n)=6/(\pi^2n^2)$ and put $Z_t=e^{-W}$ for all $t$. This is a bounded strictly positive [martingale](../../../martingale.md), but any representing driver must have $M_0=-W$, which is not integrable. Thus the unqualified claim is false under that definition. For general $Z_0$, the always-valid local-[martingale](../../../martingale.md) statement is the zero-start representation **$Z=Z_0\mathcal E(N)$**; the printed representation additionally requires the stated integrability or the convention that allows arbitrary finite initial constants.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $D=d\mathbb Q/d\mathbb P$ on $\mathcal F$. The [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) is nonnegative and $\mathbb E_{\mathbb P}D=1$. For $A\in\mathcal F_t$,

$$
\mathbb Q(A)=\mathbb E_{\mathbb P}(D\mathbf1_A)=\mathbb E_{\mathbb P}\bigl(\mathbb E_{\mathbb P}(D\mid\mathcal F_t)\mathbf1_A\bigr).
$$

Uniqueness of the restricted [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) therefore identifies

$$
\boxed{Z_t=\mathbb E_{\mathbb P}(D\mid\mathcal F_t)\geq0.}
$$

For $s\leq t$, the tower property of [conditional expectation](../../../measure-theory.md#conditional-expectation) gives $\mathbb E_{\mathbb P}(Z_t\mid\mathcal F_s)=Z_s$, and $\mathbb E_{\mathbb P}Z_t=1$. Thus $Z$ is a nonnegative true [martingale](../../../martingale.md), indeed a [uniformly integrable martingale](../../../martingale.md#uniformly-integrable-martingale), since it consists of conditional expectations of one integrable random variable. This is the [Radon-Nikodym density martingale](../../../measure-theory.md#radon-nikodym-density-martingale). Under the [usual conditions for a filtration](../../../stochastic-process.md#usual-conditions-for-a-filtration), it has the standard càdlàg version; continuity is the additional assumption in part (c), not a consequence of absolute continuity alone.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

On the finite horizon $[0,T]$, strict positivity gives equivalence of the restricted probability measures: for $A\in\mathcal F_T$, $\mathbb Q(A)=\mathbb E_{\mathbb P}(Z_T\mathbf1_A)$ vanishes if and only if $\mathbb P(A)$ vanishes. The standard change-of-measure theorem gives [semimartingale invariance under equivalent measures](../../../stochastic-calculus.md#semimartingale-invariance-under-equivalent-measures): **a process is a semimartingale under $\mathbb P$ on this horizon if and only if it is one under $\mathbb Q$**. The sample-path [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) is unchanged, but the local-[martingale](../../../martingale.md) and finite-variation parts generally change.

More explicitly, set $N=\int Z^{-1}\,dZ$, the zero-start [stochastic logarithm](../../../stochastic-calculus.md#stochastic-logarithm) of the density. For every continuous $\mathbb P$-[local martingale](../../../martingale.md#local-martingale) $L$, the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) states that

$$
\boxed{L_t^{\mathbb Q}=L_t-\int_0^t\frac{d[L,Z]_s}{Z_s}=L_t-[L,N]_t}
$$

is a continuous $\mathbb Q$-[local martingale](../../../martingale.md#local-martingale). Consequently, if the continuous [semimartingale decomposition](../../../stochastic-calculus.md#semimartingale-decomposition) under $\mathbb P$ is $X=X_0+L+V$, its decomposition under $\mathbb Q$ is

$$
X=X_0+L^{\mathbb Q}+\bigl(V+[L,N]\bigr).
$$

The covariation correction is a continuous [finite-variation process](../../../stochastic-calculus.md#finite-variation-process), locally well-defined because $Z$ stays strictly positive. In the Brownian case, if $dZ_t=Z_t\theta_t\,dB_t$, then

$$
B_t^{\mathbb Q}=B_t-\int_0^t\theta_s\,ds
$$

is a [Brownian motion](../../../brownian-motion.md) under $\mathbb Q$. The inverse finite-horizon density is $1/Z$, giving the reverse change of measure. These assertions apply on each horizon on which the density is strictly positive; they do not assert equivalence on a larger terminal sigma-algebra where the full density $D$ may vanish.

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives, for $t>0$,

$$
\mathbb P(\tau_x\leq t)=\mathbb P\left(\sup_{s\leq t}X_s\geq x\right)=2\mathbb P(X_t\geq x)=2\left(1-\Phi\left(\frac x{\sqrt t}\right)\right).
$$

For a standard [normal random variable](../../../probability-theory.md#gaussian-random-variable) $N'$, this is also $\mathbb P(|N'|\geq x/\sqrt t)=\mathbb P(x^2/(N')^2\leq t)$. Thus the [inverse-square Gaussian law of Brownian first passage](../../../markov-process.md#inverse-square-gaussian-law-of-brownian-first-passage) is

$$
\boxed{\tau_x\overset d=\frac{x^2}{(N')^2}.}
$$

In particular, $\tau_x$ is finite almost surely.

The [Brownian motions](../../../brownian-motion.md) $X,Y$ are independent, so conditional on $\tau_x=s$, the ordinate $Y_{\tau_x}$ has the same distribution as $\sqrt s\,N$, with $N$ a standard normal independent of the random time. By [Brownian scaling](../../../brownian-motion.md#brownian-scaling) and the hitting-time identity,

$$
Y_{\tau_x}\overset d=\frac{xN}{|N'|}\overset d=\frac{xN}{N'}.
$$

The last equality uses symmetry of $N$ and independence of $N,N'$: inserting the independent sign of $N'$ does not change the distribution of the numerator. Therefore

$$
\boxed{Y_{\tau_x}\overset d=xC,\qquad C\text{ standard Cauchy}.}
$$

For completeness, the ratio has density $\int_{\mathbb R}|v|\varphi(cv)\varphi(v)\,dv=1/(\pi(1+c^2))$, where $\varphi$ is the standard normal density. The scaled exit ordinate has density $x/(\pi(x^2+y^2))$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Translate the horizontal coordinate by $x$. Then $X_t+x$ is a standard [Brownian motion](../../../brownian-motion.md) starting at zero, and continuity identifies $\tau$ with its [first-passage time](../../../markov-process.md#first-passage-time) to $x$. The vertical coordinate remains an independent standard [Brownian motion](../../../brownian-motion.md) starting at zero. Part (a) therefore gives the [Cauchy exit law from a Brownian half-plane](../../../brownian-motion.md#cauchy-exit-law-from-a-brownian-half-plane):

$$
\boxed{Y_\tau\overset d=xC,\qquad f_{Y_\tau}(y)=\frac{x}{\pi(x^2+y^2)}.}
$$

The TeX transcription's initial value $-z$ and later $Y_T$ are both corrected here to the PDF's $-x$ and $Y_\tau$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Start the [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) $X_t+iY_t$ at $-x$ and stop at $\tau=\inf\{t:X_t=0\}$. The complex exponential is holomorphic with nonzero derivative. By [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion), the process $e^{X_t+iY_t}$, run on its [conformal Brownian clock](../../../brownian-motion.md#conformal-brownian-clock)

$$
A_t=\int_0^{t\wedge\tau}e^{2X_s}\,ds,
$$

is planar [Brownian motion](../../../brownian-motion.md) started at $\varepsilon=e^{-x}$, until its first exit from the unit disk. The clock is strictly increasing before $\tau$, and $A_\tau\leq\tau<\infty$ almost surely. It is legitimate to use the exponential although it is not globally injective: the Brownian coordinate brackets depend locally on the nonzero derivative, and the clock construction gives the stopped planar Brownian law. Before $\tau$, $|e^{X_t+iY_t}|<1$; at $\tau$ it equals one. Hence the disk exit time in the new clock is exactly $A_\tau$.

The continuous lifted argument of this path, starting from angle zero, is $Y_t$. Its total argument at exit is therefore $Y_\tau$, which has distribution $xC$ by part (b). If the winding count records only completed integer turns, it differs from $Y_\tau/(2\pi)$ by a remainder $R_\varepsilon$ with $|R_\varepsilon|\leq1$. If fractional turns are retained, that remainder is zero. In either convention, since $\log\varepsilon=-x$,

$$
\frac{\theta_\varepsilon}{\log\varepsilon}
=-\frac{Y_\tau}{2\pi x}-\frac{R_\varepsilon}{x}.
$$

The first term has distribution $-C/(2\pi)$ for every $x$, and the second tends to zero deterministically in absolute value as $x\to\infty$. Symmetry of the [Cauchy distribution](../../../probability-theory.md#cauchy-distribution) removes the minus sign, so [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) gives the [small-radius Brownian winding law](../../../brownian-motion.md#small-radius-brownian-winding-law):

$$
\boxed{\frac{\theta_\varepsilon}{\log\varepsilon}\ \xrightarrow[\varepsilon\downarrow0]{d}\ \frac{C}{2\pi}.}
$$

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) is constructed for the prescribed driving [Brownian motion](../../../brownian-motion.md) on the prescribed stochastic basis, adapted to the augmented filtration generated by that driver and the initial data, and satisfies the integral equation almost surely. For this equation it must be continuous, nonnegative and satisfy $Z_t=z+\int_0^t\sqrt{Z_s}\,dB_s$. [Pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) means that any two solutions on the same filtered space, with the same initial value and the same driving [Brownian motion](../../../brownian-motion.md), are indistinguishable.

The standard [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients) cannot be applied to the [square-root branching diffusion](../../../stochastic-calculus.md#square-root-branching-diffusion), because $\sigma(x)=\sqrt x$ is not Lipschitz at zero:

$$
\frac{|\sigma(h)-\sigma(0)|}{|h-0|}=\frac1{\sqrt h}\longrightarrow\infty\qquad(h\downarrow0).
$$

It is locally Lipschitz on $(0,\infty)$, which gives a solution only up to its possible approach to zero by that theorem. Thus **the missing hypothesis is the Lipschitz bound at the absorbing boundary**, not any failure of continuity. Failure of this sufficient criterion does not establish failure of strong existence or uniqueness; part (c) constructs strong existence directly.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Work on a common stochastic basis on which $B,B'$ are independent [Brownian motions](../../../brownian-motion.md) and the solutions are adapted; independent weak solutions can be put on the product stochastic basis. Independence gives $[B,B']=0$. Put $S=Z+Z'\geq0$ and define the predictable weights

$$
u_t=\begin{cases}\sqrt{Z_t/S_t},&S_t>0,\\1,&S_t=0,\end{cases}\qquad
v_t=\begin{cases}\sqrt{Z'_t/S_t},&S_t>0,\\0,&S_t=0.\end{cases}
$$

They are bounded and satisfy $u_t^2+v_t^2=1$ everywhere. Define

$$
\boxed{\beta_t=\int_0^tu_s\,dB_s+\int_0^tv_s\,dB'_s.}
$$

This is a zero-start [continuous local martingale](../../../martingale.md#continuous-local-martingale), and its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) is $[\beta]_t=\int_0^t(u_s^2+v_s^2)ds=t$. By the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion), $\beta$ is a [Brownian motion](../../../brownian-motion.md) in the common filtration.

On $\{S_t>0\}$, $\sqrt{S_t}u_t=\sqrt{Z_t}$ and $\sqrt{S_t}v_t=\sqrt{Z'_t}$. On $\{S_t=0\}$, nonnegativity forces both $Z_t,Z'_t$ to be zero, so the same identities hold. [Associativity of stochastic integration](../../../stochastic-calculus.md#associativity-of-stochastic-integration) therefore gives

$$
S_t=z+z'+\int_0^t\sqrt{S_s}\,d\beta_s.
$$

This proves the [addition law for square-root branching diffusions](../../../stochastic-calculus.md#addition-law-for-square-root-branching-diffusions): **$Z+Z'$ is a weak solution with initial value $z+z'$**. Specifying the weights at zero is necessary to keep $[\beta]_t=t$ after extinction; simply setting both weights to zero would fail to produce a Brownian driver.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For fixed $\varepsilon>0$, the derivative of $\sigma_\varepsilon$ is zero on $(-\infty,\varepsilon/2]$, bounded on the compact transition interval $[\varepsilon/2,\varepsilon]$, and equals $1/(2\sqrt x)\leq1/(2\sqrt\varepsilon)$ for $x\geq\varepsilon$. Thus $\sigma_\varepsilon$ is globally Lipschitz, with at most linear growth. The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients) supplies a global [strong stochastic solution](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) and [pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) for the modified equation.

The solution stays nonnegative. More precisely, if $z>\varepsilon/2$, it cannot cross $\varepsilon/2$: on reaching this level the constant continuation solves the equation, and [pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) forces that continuation. If $z\leq\varepsilon/2$, it is constant from the outset. In either case $Z^\varepsilon$ is a [nonnegative local martingale](../../../martingale.md#nonnegative-local-martingale), so $\mathbb E Z^\varepsilon_s\leq z$.

For $\varepsilon'<\varepsilon<z$, both coefficients agree with $\sqrt x$ on $[\varepsilon,\infty)$. Stop the two solutions when either first reaches $\varepsilon$, and also at a common upper bound. On the resulting compact state interval, the coefficient is Lipschitz. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) applied to their difference, followed by the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality), gives zero expected squared difference. Remove the upper bound using the nonexplosion of each modified solution. The two solutions agree until the first of these lower exits, and by continuity both have value $\varepsilon$ there, so their exits at that level coincide. In particular,

$$
\boxed{Z^{\varepsilon'}_t=Z^\varepsilon_t\quad(0\leq t\leq T_\varepsilon),}
$$

up to indistinguishability. If $\varepsilon\geq z$, the first exit time is zero and the same assertion is immediate from their initial values.

Now take a decreasing sequence $0<\varepsilon_n<z$ with $\varepsilon_n\downarrow0$. Write $Z^n=Z^{\varepsilon_n}$ and $\tau_n=T_{\varepsilon_n}$. Compatibility gives $\tau_n\leq\tau_{n+1}$; indeed, a continuous path cannot reach the smaller level before reaching the larger one. Let $\tau=\lim_n\tau_n$, a [stopping time](../../../martingale.md#stopping-time). On $[0,\tau)$ the compatible solutions define an adapted continuous process $Z$ by setting $Z_t=Z^n_t$ whenever $t\leq\tau_n$. We still need to justify the finite limiting endpoint and the integral equation there, rather than assume they exist.

For this purpose use the compatible predictable integrands

$$
H^n_s=\mathbf1_{\{s\leq\tau_n\}}\sqrt{Z^n_s}.
$$

Their squares increase pointwise with $n$: on the smaller interval compatibility makes the values equal, and outside it the old integrand is zero. Their limit $H$ is predictable and equals $\sqrt{Z_s}$ before $\tau$, and zero after $\tau$, apart from irrelevant single-time endpoints. For every finite $t$,

$$
\mathbb E\int_0^t(H^n_s)^2ds
=\int_0^t\mathbb E\bigl[\mathbf1_{\{s\leq\tau_n\}}Z^n_s\bigr]ds\leq zt.
$$

The [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) gives $\mathbb E\int_0^tH_s^2ds\leq zt$. Moreover, compatibility makes $(H-H^n)^2=H^2-(H^n)^2$ away from endpoints, so its expected time-integral tends to zero. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry), and the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) if uniform convergence on a finite time interval is desired, therefore give a continuous stochastic-integral limit

$$
L_t=z+\int_0^tH_s\,dB_s.
$$

Before $\tau_n$, the integrand agrees with $\sqrt{Z^n}$, which is the original square-root coefficient there. Locality of the [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) yields $L_{t\wedge\tau_n}=Z^n_{t\wedge\tau_n}$. A countable intersection in $n$ and path continuity give this equality simultaneously for all times.

On $\{\tau<\infty\}$, every $\tau_n$ is finite and $L_{\tau_n}=\varepsilon_n$. Continuity of $L$ thus gives $L_\tau=0$. The limiting integrand is zero after $\tau$, so $L$ remains zero afterward. On $\{\tau=\infty\}$, every finite time is covered by one of the compatible positive solutions. Consequently $L$ is nonnegative everywhere and $H_s=\sqrt{L_s}$ for almost every $s$, including after absorption. The [cutoff construction of an absorbed square-root diffusion](../../../stochastic-calculus.md#cutoff-construction-of-an-absorbed-square-root-diffusion) has produced

$$
\boxed{Z_t=L_t=z+\int_0^t\sqrt{Z_s}\,dB_s,\qquad Z_t=0\text{ for }t\geq\tau\text{ if }\tau<\infty.}
$$

All modified solutions, [stopping times](../../../martingale.md#stopping-time) and integrands were constructed from the same prescribed [Brownian motion](../../../brownian-motion.md); hence this is a [strong stochastic solution](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation). The integral is square-integrable on every finite horizon by the bound $zt$, which also rules out a hidden finite-time explosion in the patching argument.

## 6

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Put $R_\varepsilon=\int_0^\varepsilon(H_u-H_0)\,dB_u$ and $d_\varepsilon=\varepsilon^{-1}\int_0^\varepsilon\mathbb E|H_u-H_0|^2du$. Boundedness and path continuity of $H$ make $\mathbb E|H_u-H_0|^2\to0$ by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem), so $d_\varepsilon\to0$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives $\mathbb E R_\varepsilon^2=\varepsilon d_\varepsilon$.

We must not assume independence between the integral and its Brownian denominator. Instead, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\mathbb E\left|\frac{R_\varepsilon}{B_\varepsilon}\right|^{1/4}
\leq\bigl(\mathbb E|R_\varepsilon|^{1/2}\bigr)^{1/2}\bigl(\mathbb E|B_\varepsilon|^{-1/2}\bigr)^{1/2}.
$$

Concavity, or [Jensen inequality](../../../real-analysis.md#jensen-s-inequality), bounds the first factor by $(\mathbb E R_\varepsilon^2)^{1/8}$. Since $B_\varepsilon\overset d=\sqrt\varepsilon N$, the second factor is $\varepsilon^{-1/8}(\mathbb E|N|^{-1/2})^{1/2}$. This negative normal moment is finite: the density is bounded near zero, where $\int_0^1u^{-1/2}du<\infty$, and has Gaussian decay at infinity. In fact $\mathbb E|N|^{-1/2}=2^{-1/4}\Gamma(1/4)/\sqrt\pi$. The powers of $\varepsilon$ cancel, yielding the [fractional-moment control of Brownian increment ratios](../../../stochastic-calculus.md#fractional-moment-control-of-brownian-increment-ratios)

$$
\boxed{\mathbb E\left|\frac{R_\varepsilon}{B_\varepsilon}\right|^{1/4}\leq C d_\varepsilon^{1/8}\longrightarrow0,\qquad C=(\mathbb E|N|^{-1/2})^{1/2}.}
$$

The ratio may be assigned any value on the null event $B_\varepsilon=0$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Fix a deterministic $t>0$ and define $\widehat B_u=B_{t+u}-B_t$, $\widehat H_u=H_{t+u}$ and $\widehat{\mathcal F}_u=\mathcal F_{t+u}$. The increment process is a standard [Brownian motion](../../../brownian-motion.md) in the shifted filtration, and $\widehat H$ remains bounded, continuous and adapted. Thus part (a) applies even though the initial value $\widehat H_0=H_t$ is random. For $\varepsilon>0$,

$$
\frac{\int_t^{t+\varepsilon}H_s\,dB_s}{B_{t+\varepsilon}-B_t}-H_t
=\frac{\int_t^{t+\varepsilon}(H_s-H_t)\,dB_s}{B_{t+\varepsilon}-B_t}.
$$

Here the constant-in-time integrand $H_t$ is $\mathcal F_t$-measurable, so its [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) equals $H_t(B_{t+\varepsilon}-B_t)$. The expectation of the absolute value of the right-hand side to the power $1/4$ tends to zero by part (a). For every $\eta>0$, [Markov inequality](../../../probability-inequality.md#markov-inequality) consequently gives

$$
\mathbb P\left(\left|\frac{\int_t^{t+\varepsilon}H_s\,dB_s}{B_{t+\varepsilon}-B_t}-H_t\right|>\eta\right)
\leq\eta^{-1/4}\mathbb E\left|\frac{\int_t^{t+\varepsilon}(H_s-H_t)\,dB_s}{B_{t+\varepsilon}-B_t}\right|^{1/4}\longrightarrow0.
$$

Therefore

$$
\boxed{\frac1{B_{t+\varepsilon}-B_t}\int_t^{t+\varepsilon}H_s\,dB_s\xrightarrow[\varepsilon\downarrow0]{\mathbb P}H_t\quad\text{for every fixed }t>0.}
$$

The stated [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) holds for each fixed deterministic time.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
