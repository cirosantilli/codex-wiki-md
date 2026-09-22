# Reachability in control theory

↑ **Parent:** [Control theory](control-theory-split.md)

[Reachability in control theory](reachability-in-control-theory.md) asks about a particular initial state $x_0$ and target $x_1$: does some admissible [control input](control-input.md) make $x(T)=x_1$ at the declared time $T$, or at some allowed duration? [Controllability](controllability.md) requires this for every pair in the declared [state space](state-space.md). This is a property of state evolution, distinct from graph [reachability](reachability-in-a-graph.md).

For a [linear time-invariant system](linear-time-invariant-system.md), solving the [ordinary differential equation](ordinary-differential-equation.md) by a [matrix exponential](matrix-exponential.md) gives

$$
x(T)=e^{AT}x_0+\int_0^T e^{A(T-t)}B u(t)\,dt.
$$

The first term is the unforced endpoint. [Reachability in control theory](reachability-in-control-theory.md) asks whether the [control input](control-input.md) can supply exactly the displacement $x_1-e^{AT}x_0$. The timing matters because the same command is carried by different amounts of subsequent dynamics. [Stephen Boyd, EE263: Controllability and state transfer, slide 18–3](https://ee263.stanford.edu/archive/contr.pdf)

Here is a contrasting mathematical example with one shared [control input](control-input.md):

$$
\dot z_1=u,\qquad\dot z_2=u,\qquad
A=\begin{pmatrix}0&0\\0&0\end{pmatrix},\qquad
B=\begin{pmatrix}1\\1\end{pmatrix},\qquad
\mathcal C=\begin{pmatrix}1&0\\1&0\end{pmatrix}.
$$

The [controllability matrix](controllability-matrix.md) has [rank of a matrix](matrix-rank.md) one. Since $\frac{d}{dt}(z_1-z_2)=0$, the difference is invariant under every allowed [control input](control-input.md). From $(0,0)$ the [reachable set](reachable-set.md) is the diagonal $z_1=z_2$ when input amplitudes are unrestricted: $(1,1)$ is reachable at $T=2$ using $u=1/2$, while $(1,0)$ is impossible at every duration. Having a [control input](control-input.md) appear in both state equations did not give independent control of both states. This [reachable set](reachable-set.md) is pictured alongside the bounded [double integrator](double-integrator.md) below.

**Table of contents**

- [Reachable set](reachable-set.md)
- [Double integrator](double-integrator.md)

## ↑ Ancestors (4)

1. [Control theory](control-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Controllability Gramian](controllability-gramian.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/3/a/solution.md)
- [Reachability in control theory](reachability-in-control-theory.md)
