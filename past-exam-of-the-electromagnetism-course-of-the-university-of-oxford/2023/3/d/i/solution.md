<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $K=1/(4\pi\epsilon_0)$, $t_0=t-r/c$ and $\mathbf n=\mathbf r/r$, and evaluate $\mathbf p$, $\mathbf p'$, $\mathbf p''$ at $t_0$. The [chain rule](../../../../../chain-rule.md) gives

$$
\nabla t_0=-\frac{\mathbf n}c,\qquad
\partial_i p_j=-\frac{n_i}c p'_j,\qquad
\partial_i n_j=\frac{\delta_{ij}-n_in_j}r.
$$

In particular, for $\mathbf u(t_0)$ and any positive integer $m$,

$$
\nabla\left(\frac{\mathbf n\cdot\mathbf u}{r^m}\right)
=\frac{\mathbf u-(m+1)\mathbf n(\mathbf n\cdot\mathbf u)}{r^{m+1}}
-\frac{\mathbf n(\mathbf n\cdot\mathbf u')}{cr^m}.
$$

Apply this [gradient](../../../../../gradient.md) identity to the [electric potential](../../../../../electric-potential.md) $\phi=K[(\mathbf n\cdot\mathbf p)/r^2+(\mathbf n\cdot\mathbf p')/(cr)]$:

$$
\nabla\phi=K\left[
\frac{\mathbf p-3\mathbf n(\mathbf n\cdot\mathbf p)}{r^3}
+\frac{\mathbf p'-3\mathbf n(\mathbf n\cdot\mathbf p')}{cr^2}
-\frac{\mathbf n(\mathbf n\cdot\mathbf p'')}{c^2r}
\right].
$$

The [magnetic vector potential](../../../../../magnetic-vector-potential.md) is $\mathbf A=K\mathbf p'/(c^2r)$, with time [derivative](../../../../../derivative.md) $\partial_t\mathbf A=K\mathbf p''/(c^2r)$. Thus the [electric field](../../../../../electric-field-split.md) $\mathbf E=-\nabla\phi-\partial_t\mathbf A$ is

$$
\boxed{\mathbf E=\frac1{4\pi\epsilon_0}\left[
\frac{3\mathbf n(\mathbf n\cdot\mathbf p)-\mathbf p}{r^3}
+\frac{3\mathbf n(\mathbf n\cdot\mathbf p')-\mathbf p'}{cr^2}
+\frac{\mathbf n(\mathbf n\cdot\mathbf p'')-\mathbf p''}{c^2r}
\right].}
$$

For the [magnetic field](../../../../../magnetic-field-split.md), use the [curl](../../../../../curl.md) product rule and the [chain rule](../../../../../chain-rule.md):

$$
\begin{aligned}
\nabla\times\left(\frac{\mathbf p'}r\right)
&=\nabla(r^{-1})\times\mathbf p'+r^{-1}\nabla\times\mathbf p'\\
&=-\frac{\mathbf n\times\mathbf p'}{r^2}
-\frac{\mathbf n\times\mathbf p''}{cr}.
\end{aligned}
$$

Consequently the [fields of a time-dependent electric dipole](../../../../../fields-of-a-time-dependent-electric-dipole.md) include

$$
\boxed{\mathbf B=\frac{\mu_0}{4\pi}\left(\frac{\mathbf p'}{r^2}
+\frac{\mathbf p''}{cr}\right)\times\mathbf n.}
$$

These formulas hold for $r>0$. The $r^{-3}$ [electric field](../../../../../electric-field-split.md) is the retarded [electric dipole field](../../../../../electric-dipole-field.md), the $r^{-2}$ terms are induction contributions, and the $r^{-1}$ terms describe [electric dipole radiation](../../../../../electric-dipole-radiation.md). Retaining the dependence of $t_0$ on position in every spatial [derivative](../../../../../derivative.md) is what produces both the induction and radiation contributions.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
