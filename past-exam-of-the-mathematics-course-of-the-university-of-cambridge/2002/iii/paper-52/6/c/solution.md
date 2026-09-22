<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It is helpful to solve using the nonsingular total flux $J$ and [volume flux](../../../../../../volumetric-flow-rate.md) $Q$ before recovering $M$. The relation $J=M/(1-Q^2/(R^2M))$ is quadratic:

$$
M^2-JM+\frac{JQ^2}{R^2}=0,\qquad M=\frac{J+\sqrt{J^2-4JQ^2/R^2}}2.
$$

The plus sign selects the small-area pure-source branch. Its discriminant vanishes when $J=4Q^2/R^2$, giving

$$
\boxed{s_o=\frac12,\qquad b_o=\frac R{\sqrt2},\qquad M_o=\frac{2Q_o^2}{R^2}.}
$$

Therefore

$$
\boxed{w_o=\frac{2Q_o}{R^2},\qquad v_o=-w_o,\qquad (M_a)_o=M_o=\frac{R^2w_o^2}{2}.}
$$

The specific upward plume and ambient momentum-flux contributions are equal, not opposite. The ambient's transported [momentum](../../../../../../momentum.md) has the opposite sign from its transported volume, so their product remains positive.

To show that the pure branch actually reaches this fold in finite height and that it is a genuine pole, introduce

$$
U_* =\left(\frac{B_s}{\alpha R}\right)^{1/3},\quad q=\frac Q{R^2U_*},\quad m=\frac M{R^2U_*^2},\quad j=\frac J{R^2U_*^2},\quad \zeta=\frac{\alpha z}{R}.
$$

Then $s=q^2/m$ and

$$
\frac{dq}{d\zeta}=\frac{2\sqrt m}{1-s},\qquad \frac{dj}{dq}=\frac{q(1-s)}{2m^{3/2}},\qquad m=\frac{j+\sqrt{j^2-4jq^2}}2.
$$

The pure-source condition is $j\sim(5/8)^{2/5}q^{4/5}$. Before the fold, $s<1/2$ and $m>2q^2$. Thus for every fixed positive $q_1$, the [derivative](../../../../../../derivative.md) $dj/dq$ is bounded above by a constant times $q^{-2}$ on $q\geq q_1$. If the branch continued for arbitrarily large $q$, $j$ would remain bounded, contradicting $j\geq4q^2$. Hence it reaches $j=4q^2$ at a finite $q_o>0$. Its height is finite because $d\zeta/dq=(1-s)/(2\sqrt m)$ is finite away from the source and behaves like a constant times $q^{-2/5}$ at the source, an integrable singularity.

For the numerator, write $m=j(1-s)$. Then

$$
\frac{dj}{dq}=\frac{q}{2j^{3/2}\sqrt{1-s}}\geq\frac{q}{2j^{3/2}},\qquad j^{5/2}\geq\frac58q^2.
$$

At the fold $j=4q_o^2$, so $q_o^3\geq5/256$. On the other hand the dimensionless numerator in the $m$ equation at $s=1/2$ is

$$
\frac1{8q_o}-8\sqrt2\,q_o^2.
$$

It is strictly negative because $5/256>1/(64\sqrt2)$. The denominator $1-2s$ approaches zero from above. Consequently **$dM/dz\to-\infty$ at finite $z_o$, although the fluxes and velocities themselves remain finite**. This proves the [confined-plume momentum fold](../../../../../../confined-plume-momentum-fold.md) rather than merely noticing a possible zero denominator.

The dimensionless pure-source branch uniquely determines the remaining amplitudes. They can be specified without an elementary antiderivative by integrating the displayed scalar equation for $j(q)$ until $j=4q^2$, and setting

$$
\zeta_o=\int_0^{q_o}\frac{1-q^2/m(q)}{2\sqrt{m(q)}}\,dq.
$$

A direct numerical [integration](../../../../../../integral.md) gives $q_o\simeq0.281610$, $\zeta_o\simeq0.400049$, so the dimensional results for this specified entrainment convention are

$$
\boxed{z_o\simeq0.400049\frac R\alpha,\quad w_o\simeq0.563220\left(\frac{B_s}{\alpha R}\right)^{1/3},\quad M_o=(M_a)_o\simeq0.158608 R^2\left(\frac{B_s}{\alpha R}\right)^{2/3}.}
$$

A convention using $\alpha w$ instead of $\alpha(w-v)$ would produce different numerical amplitudes; the relative-speed convention was stated in part (a).

Physically $z_o$ is a turnover or breakdown height for a slender steady plume surrounded by uniform counterflow. The opposing streams then occupy equal areas and have equal speeds; the single-valued small-area branch cannot continue smoothly. Above it one expects lateral spreading, stronger recirculation, mixing and unsteady buoyant structures rather than a continuation of the same slender top-hat column. A detailed flow or upper-layer evolution requires restoring [pressure](../../../../../../pressure.md) and stress dynamics and, eventually, the modified ambient stratification. The model does not predict an infinite physical [velocity](../../../../../../velocity.md), nor does it require that all buoyant fluid forever remain below $z_o$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Section C](../../section-c.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
