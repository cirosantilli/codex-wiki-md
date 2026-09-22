<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Wirtinger derivatives](../../../../../wirtinger-derivatives.md) $q_z=(q_x-iq_y)/2$ and $q_{\bar z}=(q_x+iq_y)/2$. The [Laplace equation](../../../../../laplace-equation.md) gives $q_{z\bar z}=0$, so write

$$
\Phi(z)=q_z(z),\qquad q_{\bar z}(z)=\Psi(\bar z),
$$

where $\Phi$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) in the first quadrant and $\Psi$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) in the fourth quadrant. They are independent functions: the data may be complex, so a complex-conjugation relation between them cannot be assumed.

Let $\epsilon=(-1)^n$, where $\beta_1+\beta_2=n\pi/2$. The [oblique derivative boundary conditions](../../../../../oblique-derivative-boundary-condition.md) become

$$
i\bigl[e^{i\beta_1}\Phi(iy)-e^{-i\beta_1}\Psi(-iy)\bigr]=g_1(y),
\qquad e^{-i\beta_2}\Phi(x)+e^{i\beta_2}\Psi(x)=g_2(x).
$$

The hinted complementary traces would give

$$
\Phi(iy)=-\frac{e^{-i\beta_1}}2\bigl[u_1(y)+ig_1(y)\bigr],
\qquad\Phi(x)=\frac{e^{i\beta_2}}2\bigl[g_2(x)-iu_2(x)\bigr].
$$

Here $u_2$ is a function of $x>0$ on the horizontal side; the printed $y$ range in that hint is a variable typo. We shall eliminate the same unknown traces by reflection of the [holomorphic](../../../../../complex-differentiability-at-a-point.md) derivatives.

The polygonal ray formula can first be viewed as the [Cauchy integral formula](../../../../../cauchy-integral-formula.md). For an oriented edge point $\zeta$, choose its spectral ray so that $e^{ik(z-\zeta)}$ decays for interior $z$. Then

$$
\int_l e^{ik(z-\zeta)}\,dk=\frac{i}{z-\zeta}.
$$

Interchanging the edge and ray [integrals](../../../../../integral.md) in the supplied formula gives $\Phi(z)=(2\pi i)^{-1}\int_{\partial\Omega}\Phi(\zeta)/(\zeta-z)\,d\zeta$, with counterclockwise edge orientation. Thus a quadrant limit of that formula can be evaluated by the corresponding [holomorphic](../../../../../complex-differentiability-at-a-point.md) boundary jumps, provided the additional arcs at infinity and at the corner give no contribution.

Define an [holomorphic function](../../../../../holomorphic-function.md) separately in the four quadrants by

$$
H(z)=\begin{cases}
\Phi(z),&\operatorname{Re}z>0,\ \operatorname{Im}z>0,\\
e^{-2i\beta_1}\Psi(-z),&\operatorname{Re}z<0,\ \operatorname{Im}z>0,\\
-\epsilon\Phi(-z),&\operatorname{Re}z<0,\ \operatorname{Im}z<0,\\
-e^{2i\beta_2}\Psi(z),&\operatorname{Re}z>0,\ \operatorname{Im}z<0.
\end{cases}
$$

The angle condition gives $e^{2i(\beta_1+\beta_2)}=e^{-2i(\beta_1+\beta_2)}=\epsilon$. It makes the reflected definitions consistent, with parity $H(-z)=-\epsilon H(z)$. On each axis oriented outward from zero, let $J=H_{\rm left}-H_{\rm right}$. The two known boundary equations give all four jumps:

$$
\begin{array}{c|c}
\text{outward axis}&J\\\hline
x>0&e^{i\beta_2}g_2(x)\\
iy,\ y>0&i e^{-i\beta_1}g_1(y)\\
-x,\ x>0&-\epsilon e^{i\beta_2}g_2(x)\\
-iy,\ y>0&-i\epsilon e^{-i\beta_1}g_1(y).
\end{array}
$$

For example the vertical equation gives $\Phi(iy)-e^{-2i\beta_1}\Psi(-iy)=-i e^{-i\beta_1}g_1(y)$; reversing the jump order on the upward axis accounts for its displayed sign. The horizontal equation similarly supplies the positive real-axis jump, and reflection supplies the other two.

Apply the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) in the four quadrants and combine their common edges. The edge contributions are exactly the known jumps of this scalar [Riemann-Hilbert problem](../../../../../riemann-hilbert-problem.md). If the corner and large-arc [integrals](../../../../../integral.md) vanish, the representation in the first quadrant is

$$
\boxed{\Phi(z)=\frac1{2\pi i}\left[
 e^{i\beta_2}\int_0^\infty g_2(s)\left(\frac1{s-z}-\frac\epsilon{s+z}\right)ds
-e^{-i\beta_1}\int_0^\infty g_1(s)\left(\frac1{is-z}-\frac\epsilon{is+z}\right)ds\right].}
$$

This is the [rational-angle oblique derivative problem on a quadrant](../../../../../rational-angle-oblique-derivative-problem-on-a-quadrant.md) representation, with all unknown traces removed. The Cauchy [integrals](../../../../../integral.md) have precisely the displayed jumps by the [Sokhotski–Plemelj formula](../../../../../sokhotski-plemelj-theorem.md). Their reflection parity then reconstructs $\Psi$ from the fourth-quadrant value of $H$, so the two original boundary equations hold. Integrating $\Phi(z)$ and $\Psi(\bar z)$ gives a [harmonic function](../../../../../harmonic-function.md) $q$ up to an additive constant.

To put the answer back on the spectral rays of the question, define

$$
\widehat g_2(k)=\int_0^\infty e^{-iks}g_2(s)\,ds,
\qquad \widehat g_1(k)=\int_0^\infty e^{ks}g_1(s)\,ds.
$$

Use $1/(s-z)=i\int_0^\infty e^{ik(z-s)}\,dk$, $1/(s+z)=-i\int_0^\infty e^{ik(z+s)}\,dk$, and the same identities with $s$ replaced by $is$ and the ray $0\to i\infty$. The spectral representation is

$$
\boxed{q_z(z)=\frac{e^{i\beta_2}}{2\pi}\int_0^\infty e^{ikz}\bigl[\widehat g_2(k)+\epsilon\widehat g_2(-k)\bigr]dk
-\frac{e^{-i\beta_1}}{2\pi}\int_0^{i\infty}e^{ikz}\bigl[\widehat g_1(k)+\epsilon\widehat g_1(-k)\bigr]dk.}
$$

All transforms used on these rays are ordinary boundary values of convergent half-line transforms. For $z=x+iy$ with $x,y>0$, the real-ray [integrand](../../../../../integrand.md) decays through $e^{-ky}$ and the imaginary-ray [integrand](../../../../../integrand.md) through $e^{-\operatorname{Im}k\,x}$.

There is an admissibility qualification in passing from a bounded polygon to this unbounded quadrant. Sufficient conditions are $H(z)\to0$ at infinity uniformly away from the axes, with the corresponding large-arc [integral](../../../../../integral.md) tending to zero, and $|z|H(z)\to0$ uniformly on small corner arcs. The latter allows logarithmic gradient singularities but excludes a pole with nonzero corner contribution. Smooth decaying data alone, as printed, do not impose these conditions on $q$.

For a concrete [homogeneous corner ambiguity in a quadrant Laplace problem](../../../../../homogeneous-corner-ambiguity-in-a-quadrant-laplace-problem.md), with $\beta_1=\beta_2=0$ and zero data, $q=xy$ satisfies both prescribed tangential derivative conditions but has $q_z=-iz/2$, while the displayed particular representation is zero. With $\beta_1=\beta_2=\pi/2$, the zero-data solution $q=\log|z|$ has $q_z=1/(2z)$: it decays at infinity but has an excluded corner pole. Thus no unique representation of every unrestricted solution follows from the printed data alone. Without the arc conditions, one must add a homogeneous [holomorphic](../../../../../complex-differentiability-at-a-point.md) term $P(z)$ to the displayed $q_z$, with reflected parity $P(-z)=-\epsilon P(z)$; permitted corner singularities are included if the admissible class allows them. With the stated decay and corner conditions that term vanishes, giving the boxed formulas. This identifies the missing solution-class conditions without assuming real-valued data.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
