<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [contact process](../../../../../contact-process.md) convention that each infected [vertex](../../../../../vertex-graph-theory.md) recovers at rate one and sends infection arrows to each neighbour at rate $\lambda$. Starting from a finite set, the process stays finite and is nonexplosive: its total birth rate is at most $\lambda(d+1)$ times its current size, so a linear-rate [branching process](../../../../../branching-process.md) dominates the number of births. The bound involving $(d-1)^{-1}$ presupposes the branching-tree case $d\ge2$.

For a nonempty finite infected set $A$, put $a=|A|$, let $e(A)$ count its internal [edges](../../../../../edge-of-a-graph.md), and let $b(A)$ count [edges](../../../../../edge-of-a-graph.md) with exactly one endpoint in $A$. Each such boundary [edge](../../../../../edge-of-a-graph.md) contributes infection rate $\lambda$, even when several lead to the same vacant [vertex](../../../../../vertex-graph-theory.md). Since the induced [graph](../../../../../graph-split.md) is a [forest](../../../../../forest.md), $e(A)\le a-1$, and the [edge boundary of a finite forest in a regular tree](../../../../../edge-boundary-of-a-finite-forest-in-a-regular-tree.md) gives

$$
b(A)=(d+1)a-2e(A)\ge(d-1)a+2.
$$

A recovery multiplies $\nu_\rho(A)=\rho^a$ by $\rho^{-1}$, while an infection multiplies it by $\rho$. Therefore its [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) is

$$
L\nu_\rho(A)=a(\rho^{a-1}-\rho^a)+\lambda b(A)(\rho^{a+1}-\rho^a)
=(1-\rho)\nu_\rho(A)\left(\frac a\rho-\lambda b(A)\right).
$$

Substituting the boundary lower bound gives

$$
\boxed{\left.\frac{d}{dt}\mathbb E_\lambda\nu_\rho(\xi_t^A)\right|_{t=0}
\le(1-\rho)\nu_\rho(A)\left[\frac{|A|}{\rho}\bigl(1-\lambda\rho(d-1)\bigr)-2\lambda\right]}.
$$

At the absorbing empty set the generator is zero, rather than this nonempty-set expression. If $\lambda\rho(d-1)\ge1$, the generator is nonpositive in every state. Both $\nu_\rho$ and its generator are bounded, since $a\rho^a$ is bounded and $b(A)\le(d+1)a$. Applying [Dynkin's formula](../../../../../dynkin-s-formula.md) over successive time intervals with the [Markov property](../../../../../markov-property.md) proves the [exponential cardinality supermartingale for the contact process on a tree](../../../../../exponential-cardinality-supermartingale-for-the-contact-process-on-a-tree.md). In particular,

$$
\boxed{t\longmapsto\mathbb E_\lambda\nu_\rho(\xi_t^A)\text{ is non-increasing}}.
$$

If $\tau$ is the extinction time, $\mathbf1_{\{\tau\le t\}}\le\nu_\rho(\xi_t^A)$, so $\mathbb P_\lambda(\tau<\infty)\le\rho^{|A|}<1$. Choosing $\rho\in[1/(\lambda(d-1)),1)$ proves global survival whenever $\lambda>1/(d-1)$. Obtaining a strict improvement of the threshold requires an additional comparison.

Here is a [two-vertex branching comparison for contact-process survival](../../../../../two-vertex-branching-comparison-for-contact-process-survival.md). Delete one [edge](../../../../../edge-of-a-graph.md) incident to a starting [vertex](../../../../../vertex-graph-theory.md) and retain its forward rooted subtree, so every [vertex](../../../../../vertex-graph-theory.md) has $d$ children. Partition it into cells as follows: pair each cell root $u$ with one distinguished child $v$; the other $d-1$ children of $u$ and all $d$ children of $v$ become roots of child cells, and repeat recursively. Each cell thus has $2d-1$ child cells.

Suppress arrows back from a child cell into its parent, allow each child cell to be activated only once, and let infection inside each two-[vertex](../../../../../vertex-graph-theory.md) cell evolve with the usual recoveries and reinfections until both [vertices](../../../../../vertex-graph-theory.md) are healthy. A child cell is activated at its root by the first outgoing arrow to it while the corresponding parent [vertex](../../../../../vertex-graph-theory.md) is infected. This process is contained in the original infection process under the [graphical representation of the contact process](../../../../../graphical-representation-of-the-contact-process.md): only infection paths have been removed. The Poisson clocks inside a child cell and on its outgoing [edges](../../../../../edge-of-a-graph.md) have not previously been used. The [Strong Markov property](../../../../../strong-markov-property.md) and [independence](../../../../../independent-random-variables.md) of the clocks therefore make different cells' offspring counts independent and identically distributed. Dependence among different children of the same cell does not matter. The cell genealogy is a [Galton-Watson process](../../../../../galton-watson-process.md).

Let $a$ be the [probability](../../../../../probability.md) that a cell, initially infected only at $u$, sends an arrow along one specified outgoing [edge](../../../../../edge-of-a-graph.md) from $u$ before internal extinction. Let $b$ be the corresponding [probability](../../../../../probability.md) for one specified outgoing [edge](../../../../../edge-of-a-graph.md) from $v$, and let $c$ be the [probability](../../../../../probability.md) of success for the first target when both cell [vertices](../../../../../vertex-graph-theory.md) are initially infected. First-step conditioning on the three nonempty pair states gives

$$
(1+2\lambda)a=\lambda c+\lambda,\qquad
(1+\lambda)b=\lambda c,\qquad
(2+\lambda)c=a+b+\lambda.
$$

For example, from the state with only $u$ infected, recovery at rate one fails, an internal arrow at rate $\lambda$ leads to the two-infected state, and the target arrow at rate $\lambda$ succeeds. From the state with only $v$ infected, the target cannot be reached until $u$ is infected. Symmetry identifies this latter success [probability](../../../../../probability.md) with $b$. Solving these equations yields

$$
a=\frac{2\lambda^3+3\lambda^2+2\lambda}{D},\qquad
b=\frac{2\lambda^3+2\lambda^2}{D},\qquad
D=2\lambda^3+4\lambda^2+5\lambda+2.
$$

By [linearity of expectation](../../../../../linearity-of-expectation.md), the offspring mean is $M(\lambda)=(d-1)a+db$. At the comparison rate $\lambda_0=1/(d-1)$,

$$
\boxed{M(\lambda_0)-1=\frac{2(d-1)}{2d^3-d^2+1}>0}.
$$

These finite-state [probabilities](../../../../../probability.md) are continuous in $\lambda$. Hence some $0<\lambda'<\lambda_0$ still has $M(\lambda')>1$. The [branching-process extinction criterion](../../../../../branching-process-extinction-criterion.md) gives positive [probability](../../../../../probability.md) of infinitely many activated cells. Nonexplosion prevents infinitely many activations in bounded time, and each activation is connected to its ancestor by an infection path. Thus infection survives for all time on that event. The [global survival threshold of the contact process](../../../../../global-survival-threshold-of-the-contact-process.md) consequently satisfies

$$
\boxed{\lambda_1\le\lambda'<\frac1{d-1}}.
$$

Retaining reinfection inside pairs is what supplies the strict improvement; a comparison that permits only one infection per [vertex](../../../../../vertex-graph-theory.md) would give merely the non-strict bound.

For the local-survival estimate, set $h(x)=\rho^{g(x)}$ and $w_\rho(A)=\sum_{x\in A}h(x)$. Each [vertex](../../../../../vertex-graph-theory.md) has one neighbour of weight $\rho^{-1}h(x)$ and $d$ neighbours of weight $\rho h(x)$. Recoveries remove their [vertex](../../../../../vertex-graph-theory.md) weights. Ignoring the restriction that an infection target must be vacant only increases the birth contribution, so

$$
\begin{aligned}
Lw_\rho(A)
&=-\sum_{x\in A}h(x)+\lambda\sum_{x\in A}\sum_{y\sim x,\ y\notin A}h(y)\\
&\le\bigl[-1+\lambda(\rho^{-1}+d\rho)\bigr]w_\rho(A).
\end{aligned}
$$

These weights have finite [expectations](../../../../../expected-value.md) on finite time intervals: a birth-only [branching process](../../../../../branching-process.md) with the same spatial arrows has expected weight at most $w_\rho(A)e^{\lambda(\rho^{-1}+d\rho)t}$. This justifies localization and the [expectation](../../../../../expected-value.md) identity for the generator. If $c=1-\lambda(\rho^{-1}+d\rho)>0$, [Dynkin's formula](../../../../../dynkin-s-formula.md) and the integrating-factor form of the [Gronwall inequality](../../../../../gronwall-inequality.md) give

$$
\mathbb E_\lambda w_\rho(\xi_t^A)\le e^{-ct}w_\rho(A).
$$

For $d\ge2$, take $\rho=d^{-1/2}$, which minimizes $\rho^{-1}+d\rho$ and makes it $2\sqrt d$. Starting from $\{x\}$ then gives

$$
\boxed{\mathbb P_\lambda(x\in\xi_t^{\{x\}})
\le\frac{\mathbb E_\lambda w_\rho(\xi_t^{\{x\}})}{h(x)}
\le e^{-(1-2\lambda\sqrt d)t}\qquad\left(\lambda<\frac1{2\sqrt d}\right)}.
$$

In particular the expected total occupation time of $x$ is finite. Its recovery clock has rate one, so the expected number of recovery marks that occur while $x$ is infected equals this occupation-time integral and is finite. Each infection episode ends almost surely at a recovery. Infection at unbounded times would therefore require infinitely many such recoveries, an event of [probability](../../../../../probability.md) zero. This [height-weighted local extinction bound for the contact process](../../../../../height-weighted-local-extinction-bound-for-the-contact-process.md) proves

$$
\boxed{\lambda_2\ge\frac1{2\sqrt d}}.
$$

This is a bound for the [local survival threshold of the contact process](../../../../../local-survival-threshold-of-the-contact-process.md), not just a bound on single-time infection [probabilities](../../../../../probability.md). For the degree-two tree $d=1$, the same local conclusion follows by choosing $\rho<1$ sufficiently close to one for each $\lambda<1/2$; the displayed expression $1/(d-1)$ for the global threshold is not a finite numerical assertion in that case.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
