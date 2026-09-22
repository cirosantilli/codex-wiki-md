<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $w=\dot v$. The planar [vector field](../../../../../../vector-field.md) and its [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) [eigenvalue](../../../../../../eigenvalue.md) data are

$$
\dot v=w,\qquad\dot w=-\lambda v+2\varepsilon v^2+v^3+(\kappa-v^2)w,
$$



$$
v_0=0,\quad v_\pm=-\varepsilon\pm\sqrt{\varepsilon^2+\lambda},\qquad
\operatorname{tr}J=\kappa-v_*^2,\quad\det J=\lambda-4\varepsilon v_*-3v_*^2.
$$

For a nonzero [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md), use $\lambda=v_*^2+2\varepsilon v_*$ to rewrite the [determinant](../../../../../../determinant.md) as $-2v_*(v_*+\varepsilon)$. These formulas determine the local bifurcations of the [imperfect soft Duffing-van der Pol oscillator](../../../../../../imperfect-soft-duffing-van-der-pol-oscillator.md) directly.

When $\varepsilon=0$, the origin is a [saddle equilibrium](../../../../../../saddle-equilibrium.md) for $\lambda<0$ and has [determinant](../../../../../../determinant.md) $\lambda$ for $\lambda>0$; the two [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) $\pm\sqrt\lambda$ are [saddle equilibria](../../../../../../saddle-equilibrium.md). They meet the origin in a symmetry-protected [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) at $\lambda=0$ for $\kappa\ne0$. At $\kappa=0,\lambda>0$ the origin undergoes a [supercritical Hopf bifurcation](../../../../../../supercritical-hopf-bifurcation.md). To determine criticality, take $v=r\cos(\sqrt\lambda t)+\cdots$: averaging $\dot H=(\kappa-v^2)w^2$ gives $\dot r=\kappa r/2-r^3/8+\cdots$, so the stable small [limit cycle](../../../../../../limit-cycle.md) has $r^2=4\kappa+\cdots$.

The [potential energy](../../../../../../potential-energy.md) of the conservative part and the exact [energy](../../../../../../energy.md) balance are

$$
H=\frac12w^2+\frac12\lambda v^2-\frac23\varepsilon v^3-\frac14v^4,
\qquad\dot H=(\kappa-v^2)w^2.
$$

At zero imperfection the stable [limit cycle](../../../../../../limit-cycle.md) grows to a [heteroclinic cycle](../../../../../../heteroclinic-cycle.md) connecting the two outer [saddle equilibria](../../../../../../saddle-equilibrium.md). Near the double-zero point its leading connection curve can be calculated, rather than inferred just from symmetry. In the [Hamiltonian system](../../../../../../hamiltonian-system.md) limit the [heteroclinic orbit](../../../../../../heteroclinic-orbit.md) is $v=\sqrt\lambda\tanh(\sqrt{\lambda/2}\,t)$, and

$$
\int_{-\infty}^{\infty}w^2dt=\frac{4\lambda^{3/2}}{3\sqrt2},\qquad
\frac{\int v^2w^2dt}{\int w^2dt}=\frac\lambda5.
$$

The weak-damping persistence condition is therefore $\kappa=\lambda/5+o(\lambda)$, not an exact formula at order-one parameters.

Now take $\varepsilon>0$; negative imperfection reflects the phase portrait. The [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) unfolds into **a [transcritical bifurcation](../../../../../../transcritical-bifurcation.md) crossing at $\lambda=0$ and a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) at $\lambda=-\varepsilon^2$**. The latter occurs at $v=-\varepsilon$. Between those values the origin and $v_-$ are [saddle equilibria](../../../../../../saddle-equilibrium.md), while $v_+$ lies in $(-\varepsilon,0)$ and is a sink or source according to the [trace](../../../../../../matrix-trace.md). At $\lambda=0$, $v_+=\lambda/(2\varepsilon)+\cdots$ exchanges its [saddle equilibrium](../../../../../../saddle-equilibrium.md)/non-saddle character with the origin. The double-zero points are now at $(\lambda,\kappa)=(0,0)$ and $(-\varepsilon^2,\varepsilon^2)$.

The original [Hopf bifurcation](../../../../../../hopf-bifurcation.md) line $\kappa=0,\lambda>0$ remains, still supercritical. A second [Hopf bifurcation](../../../../../../hopf-bifurcation.md) curve occurs on the intermediate nonzero [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md):

$$
\boxed{\lambda=q^2+2\varepsilon q,\quad\kappa=q^2,\quad-\varepsilon<q<0.}
$$

It is important not to assign the same criticality to its entire length. Write $s=\sqrt{\varepsilon^2+\lambda}$, so $q=-\varepsilon+s$. Around that center the restoring quadratic coefficient is $g_2=-\varepsilon+3s$, the damping linear coefficient is $f_1=2(\varepsilon-s)$, and $\omega^2=2s(\varepsilon-s)$. The [Hopf criticality for an asymmetric Lienard center](../../../../../../hopf-criticality-for-an-asymmetric-lienard-center.md) calculation gives cubic amplitude coefficient

$$
\frac18\left(-1+\frac{f_1g_2}{\omega^2}\right)=\frac18(2-\varepsilon/s).
$$

Hence it is supercritical for $s<\varepsilon/2$ and subcritical for $s>\varepsilon/2$, with a [generalized Hopf bifurcation](../../../../../../generalized-hopf-bifurcation.md) point at $\lambda=-3\varepsilon^2/4,\kappa=\varepsilon^2/4$. Higher-order terms are needed exactly there. For small imperfection the leading quintic coefficient is positive: writing $q_1=v-q$ and using the coordinate that normalizes the [potential energy](../../../../../../potential-energy.md), $y=q_1\sqrt{1-aq_1-bq_1^2}$, with $a=2g_2/(3\omega^2)$ and $b=1/(2\omega^2)$, the coefficient of $y^4$ in $(f_1q_1-q_1^2)dq_1/dy$ at vanishing cubic coefficient is $10b/3>0$. Weak-damping averaging therefore supplies the nearby [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) of stable and unstable [limit cycles](../../../../../../limit-cycle.md) in the [generalized Hopf bifurcation](../../../../../../generalized-hopf-bifurcation.md) unfolding. None of these small $O(\varepsilon^2)$ features intersects either requested parameter line.

Globally, the two [saddle equilibrium](../../../../../../saddle-equilibrium.md) barriers are no longer equal. Their leading [energy](../../../../../../energy.md) difference is $H(v_+,0)-H(v_-,0)=-4\varepsilon\lambda^{3/2}/3+\cdots$. The two one-way connections consequently separate; matching their [energy](../../../../../../energy.md) differences with the connection integral gives

$$
\kappa=\lambda/5-\sqrt2\,\varepsilon+\cdots\quad(v_-\to v_+),\qquad
\kappa=\lambda/5+\sqrt2\,\varepsilon+\cdots\quad(v_+\to v_-).
$$

These [weak-damping heteroclinic splitting of a tilted quartic oscillator](../../../../../../weak-damping-heteroclinic-splitting-of-a-tilted-quartic-oscillator.md) formulas apply for small $\lambda$ with $|\varepsilon|\ll\sqrt\lambda$. Between the separated connection curves, the central stable [limit cycle](../../../../../../limit-cycle.md) terminates in a [homoclinic orbit](../../../../../../homoclinic-orbit.md) to the lower-barrier [saddle equilibrium](../../../../../../saddle-equilibrium.md), $v_+$ for positive imperfection. The simultaneous symmetric heteroclinic-cycle destruction is therefore replaced by two basin-changing one-way connections and a distinct [homoclinic orbit](../../../../../../homoclinic-orbit.md) loss of the [limit cycle](../../../../../../limit-cycle.md). Its period diverges at that loss.

Along $\kappa+\lambda=1$, decrease $\lambda$ from above one. The sequence is **[supercritical Hopf bifurcation](../../../../../../supercritical-hopf-bifurcation.md) at $\lambda=1$; first [heteroclinic orbit](../../../../../../heteroclinic-orbit.md); [homoclinic orbit](../../../../../../homoclinic-orbit.md) loss of the stable [limit cycle](../../../../../../limit-cycle.md); second [heteroclinic orbit](../../../../../../heteroclinic-orbit.md); [transcritical bifurcation](../../../../../../transcritical-bifurcation.md) crossing at zero; [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) at $-\varepsilon^2$**. The connection locations are global, not obtained by treating the Melnikov approximation as exact. For illustration, direct stable/unstable manifold matching at $\varepsilon=0.04$ places them at approximately $\lambda=0.882,0.858,0.783$, respectively. The diagram below gives the qualitative ordering without prescribing those example values for arbitrary imperfection.

Along $\kappa+\lambda=-1$, the sequence is simply **[transcritical bifurcation](../../../../../../transcritical-bifurcation.md) crossing at zero, followed by [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) at $-\varepsilon^2$**. Before the latter, $\kappa<0$ in the relevant region, so $H$ decreases strictly on nonstationary trajectories and there is no [periodic orbit](../../../../../../periodic-orbit.md) or [saddle equilibrium](../../../../../../saddle-equilibrium.md) loop. After it only a [saddle equilibrium](../../../../../../saddle-equilibrium.md) remains, which cannot be enclosed by a [periodic orbit](../../../../../../periodic-orbit.md) by the [Poincare-index obstruction to a periodic orbit](../../../../../../poincare-index-obstruction-to-a-periodic-orbit.md). The origin does not undergo a [Hopf bifurcation](../../../../../../hopf-bifurcation.md) at $\lambda=-1$, since its [determinant](../../../../../../determinant.md) there is negative.

<a id="2/b/image-bifurcation-sequences-along-the-two-diagonal-parameter-lines-after-a-small-positive-reflection-symmetry-imperfection-arrows-indicate-decreasing-lambda"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-60-oscillator-sequences.png)

**[Figure 2](#2/b/image-bifurcation-sequences-along-the-two-diagonal-parameter-lines-after-a-small-positive-reflection-symmetry-imperfection-arrows-indicate-decreasing-lambda). Bifurcation sequences along the two diagonal parameter lines after a small positive reflection-symmetry imperfection; arrows indicate decreasing lambda**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
