<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

A transformation of [phase space](../../../../../phase-space.md) is [canonical](../../../../../canonical-transformation.md) when it preserves the [symplectic form](../../../../../symplectic-form.md), or equivalently all [Poisson brackets](../../../../../poisson-bracket.md). For one degree of freedom this is

$$
dQ\wedge dP=dq\wedge dp,
$$

equivalently $\{Q,P\}_{q,p}=1$.

Suppose a [type-two generating function for a canonical transformation](../../../../../type-two-generating-function-for-a-canonical-transformation.md) $F(q,P)$ defines

$$
p=F_q,
\qquad Q=F_P.
$$

Then

$$
\begin{aligned}
dq\wedge dp&=F_{qP}\,dq\wedge dP,\\
dQ\wedge dP&=F_{Pq}\,dq\wedge dP.
\end{aligned}
$$

Equality of the mixed partial derivatives gives $dq\wedge dp=dQ\wedge dP$, so the transformation is canonical wherever it is locally invertible.

For

$$
F_0(q,P)=\int_0^q\sqrt{2P-u^2}\,du,
$$

the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) and differentiation under the integral sign give

$$
p=\sqrt{2P-q^2},
\qquad
Q=\int_0^q\frac{du}{\sqrt{2P-u^2}}
=\arcsin\frac{q}{\sqrt{2P}}.
$$

Thus

$$
q=\sqrt{2P}\sin Q,
\qquad
p=\sqrt{2P}\cos Q,
$$

and in particular $P=(p^2+q^2)/2$.

For the unit-frequency [simple harmonic motion](../../../../../simple-harmonic-motion.md), the transformed [Hamiltonian](../../../../../hamiltonian.md) is simply $H=P$. [Hamilton's equations](../../../../../hamilton-s-equations.md) become

$$
\dot Q=\frac{\partial H}{\partial P}=1,
\qquad
\dot P=-\frac{\partial H}{\partial Q}=0.
$$

Therefore

$$
P(t)=E,
\qquad Q(t)=t-t_0,
$$

and transformation back gives the familiar solution

$$
q(t)=\sqrt{2E}\sin(t-t_0),
\qquad
p(t)=\sqrt{2E}\cos(t-t_0).
$$

Now consider the weak [quartic oscillator](../../../../../quartic-oscillator.md)

$$
H(q,p)=\frac12(p^2+q^2)+\epsilon q^4.
$$

Choose the modified generating function

$$
F_\epsilon(q,P)
=\int_0^q\sqrt{2P-u^2-2\epsilon u^4}\,du.
$$

It gives

$$
p=\sqrt{2P-q^2-2\epsilon q^4},
$$

so the transformed Hamiltonian is again $H=P$. Hence $P=E$ and $Q=t-t_0$. Expanding the square root with the [Taylor series](../../../../../taylor-series.md) gives

$$
F_\epsilon(q,P)
=F_0(q,P)
-\epsilon\int_0^q\frac{u^4}{\sqrt{2P-u^2}}\,du
+O(\epsilon^2).
$$

Differentiation with respect to $P$ therefore yields

$$
Q
=\arcsin\frac{q}{\sqrt{2P}}
+\epsilon I(q,P)+O(\epsilon^2),
$$

where

$$
I(x,y)=\int_0^x\frac{u^4}{(2y-u^2)^{3/2}}\,du.
$$

Set $\theta=t-t_0$ and

$$
q_0=\sqrt{2E}\sin\theta,
\qquad
p_0=\sqrt{2E}\cos\theta.
$$

Writing $q=q_0+\epsilon q_1+O(\epsilon^2)$ and expanding the [inverse sine](../../../../../inverse-sine.md) relation at $q_0$ gives

$$
0=\frac{q_1}{p_0}+I(q_0,E),
\qquad
q_1=-p_0I(q_0,E).
$$

Expanding $p^2=2E-q^2-2\epsilon q^4$ similarly gives

$$
p=p_0+\epsilon p_1+O(\epsilon^2),
\qquad
p_1=q_0I(q_0,E)-\frac{q_0^4}{p_0}.
$$

Consequently

$$
\begin{aligned}
\frac qp
&=\frac{q_0}{p_0}
 +\epsilon\left(\frac{q_1}{p_0}
 -\frac{q_0p_1}{p_0^2}\right)
 +O(\epsilon^2)\\
&=\tan\theta
 -\epsilon I(q_0,E)(1+\tan^2\theta)
 +\epsilon q_0^2\tan^3\theta
 +O(\epsilon^2).
\end{aligned}
$$

Since $\theta=t-t_0$, this is the required expression. The formula is understood away from turning points where $p_0=0$ and the ratio $q/p$ itself is singular.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
