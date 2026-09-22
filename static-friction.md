# Static friction

↑ **Parent:** [Force](force-split.md)

[Static friction](static-friction.md) is the tangential contact [force](force-split.md) that maintains zero [contact slip](contact-slip.md). “Static” describes the contact state: both surfaces can move together in the chosen [inertial frame](inertial-frame.md). In the ideal dry-contact model, the actual [static friction](static-friction.md) adjusts to the [equations of motion](equation-of-motion.md), subject to a bound, rather than always taking its maximum value.[Static and Kinetic Friction; Magnitude of Static Friction, equation 6.1 and responsive-force paragraph](university-physics-volume-1-by-william-moebs-and-others/6-2-friction.md)

$$
|f_s|\le\mu_sN,\qquad N\ge0,\quad\mu_s\ge0.
$$

Here $N$ is the magnitude of the [normal force](normal-force.md) and $\mu_s$ the [coefficient of static friction](coefficient-of-static-friction.md). Equality means limiting [static friction](static-friction.md); it is a threshold, not an instruction to replace every unknown contact [force](force-split.md) by $\mu_sN$.

For a stipulated example, place a nonrotating $2\,\mathrm{kg}$ block initially at rest on a stationary horizontal surface. Take [gravitational acceleration](gravitational-acceleration.md) $g=9.8\,\mathrm{m/s^2}$ and [coefficient of static friction](coefficient-of-static-friction.md) $\mu_s=0.40$, with no other vertical [force](force-split.md). The vertical [force balance](force-balance.md) gives $N=mg=19.6\,\mathrm N$, so the largest allowed [static friction](static-friction.md) magnitude is $7.84\,\mathrm N$. Choose right as positive and apply a horizontal [force](force-split.md) $F$. Remaining at rest requires [Newton's second law](newton-s-second-law.md) to give

$$
F+f_s=0,\qquad f_s=-F,\qquad |F|\le7.84\,\mathrm N.
$$

At $F=2\,\mathrm N$, the [static friction](static-friction.md) is $-2\,\mathrm N$; at $F=6\,\mathrm N$, it is $-6\,\mathrm N$. Both states have zero [acceleration](acceleration.md). At $F=10\,\mathrm N$, balancing would require $f_s=-10\,\mathrm N$, outside the bound, so this initially resting block cannot remain at rest. Its subsequent [acceleration](acceleration.md) requires a [kinetic friction](kinetic-friction.md) law; setting $f_s=-7.84\,\mathrm N$ after [contact slip](contact-slip.md) begins would still use the wrong contact state. At exactly $F=7.84\,\mathrm N$, the ideal inequality still permits rest at the threshold. These are model calculations, not measured material properties.

<a id="image-static-friction-adjusts-to-the-applied-force-within-its-admissible-bound"></a>
![](static-friction-adjustable-response.png)

**[Figure 1](#image-static-friction-adjusts-to-the-applied-force-within-its-admissible-bound). Static friction adjusts to the applied force within its admissible bound**. Original signed horizontal model for the stipulated $2\,\mathrm{kg}$ block: the shaded band is the allowed [static friction](static-friction.md), the solid line satisfies [force balance](force-balance.md), and the dashed line shows the demand outside that band. The crossed points at $F=\pm10\,\mathrm N$ are impossible static demands, not sliding [forces](force-split.md).

The toy model used in [kinetic friction](kinetic-friction.md) makes the contact-state distinction explicit: $m=1\,\mathrm{kg}$, $N=10\,\mathrm N$, $\mu_s=0.5$ and [coefficient of kinetic friction](coefficient-of-kinetic-friction.md) $\mu_k=0.3$. On stationary ground, an initially resting box pushed right with $4\,\mathrm N$ has $f_s=-4\,\mathrm N$. At $6\,\mathrm N$ it cannot remain at rest; once it slides right, $f_k=-3\,\mathrm N$ and $a=3\,\mathrm{m/s^2}$. At $5\,\mathrm N$, rest is allowed with $f_s=-5\,\mathrm N$, whereas an already right-sliding box has $f_k=-3\,\mathrm N$ and $a=2\,\mathrm{m/s^2}$. The applied [force](force-split.md) alone does not specify the [friction](friction.md) branch: [contact slip](contact-slip.md) and motion history matter.

For a flat contact with two tangential directions, the bound applies to a [vector norm](norm.md), not separately to each component:

$$
\|\mathbf f_s\|\le\mu_sN,\qquad
f_{s,x}^{\,2}+f_{s,y}^{\,2}\le(\mu_sN)^2.
$$

For the stipulated $7.84\,\mathrm N$ bound, balancing horizontal components $4\,\mathrm N$ and $4\,\mathrm N$ requires a [force](force-split.md) magnitude $\sqrt{32}\,\mathrm N\simeq5.657\,\mathrm N$, which is allowed. Components $6\,\mathrm N$ and $6\,\mathrm N$ require $\sqrt{72}\,\mathrm N\simeq8.485\,\mathrm N$, which is forbidden even though each component separately is below $7.84\,\mathrm N$. This circular bound assumes the same [coefficient of static friction](coefficient-of-static-friction.md) in every tangential direction. Near impending [contact slip](contact-slip.md), the limiting [static friction](static-friction.md) opposes the relative contact motion that would otherwise begin. Once actual [contact slip](contact-slip.md) exists, [kinetic friction](kinetic-friction.md) instead opposes its tangential [relative velocity](relative-velocity.md), which need not have the direction of the body's [center of mass](center-of-mass.md) motion.

The [normal force](normal-force.md) must also come from the [equations of motion](equation-of-motion.md). On horizontal ground, an upward pull of magnitude $P$ at [angle](angle.md) $\alpha$ above horizontal gives, for a block remaining at rest with no other [forces](force-split.md),

$$
N=mg-P\sin\alpha,\qquad f_s=-P\cos\alpha,\qquad
|P\cos\alpha|\le\mu_s(mg-P\sin\alpha).
$$

The [sine](sine.md) component unloads the contact and the [cosine](cosine.md) component demands tangential support. These equations require $N>0$; if the supporting contact opens, this dry-contact model cannot supply a negative [normal force](normal-force.md). For the stipulated $2\,\mathrm{kg}$ block and $\alpha=30^\circ$, the positive threshold is $P=\mu_smg/(\cos\alpha+\mu_s\sin\alpha)\simeq7.3544\,\mathrm N$, with $N\simeq15.9228\,\mathrm N$ and $|f_s|\simeq6.3691\,\mathrm N$. A downward pull increases $N$ instead. An [inclined plane](inclined-plane.md) gives another reason why $N$ is not always $mg$.

To solve a new problem, impose zero [contact slip](contact-slip.md), find the required [static friction](static-friction.md) and [normal force](normal-force.md) from the [equations of motion](equation-of-motion.md), then check the bound. A demand inside it permits that contact state; a demand outside it rules the state out. For an ideal driven tire undergoing [rolling without slipping](rolling-without-slipping.md) on stationary ground, a forward [static friction](static-friction.md) can accelerate the vehicle. Its role is to prevent [contact slip](contact-slip.md), rather than to oppose all motion of the whole body.

Nor does the word “static” by itself make [friction](friction.md) do zero [work](work.md). The contact [power](power.md) delivered to a body is $P_s=\mathbf f_s\cdot\mathbf v_c$, a [dot product](dot-product.md) with its material contact-point [velocity](velocity.md) in the chosen [inertial frame](inertial-frame.md). At an ideal contact undergoing [rolling without slipping](rolling-without-slipping.md) on stationary ground, $\mathbf v_c=\mathbf0$, so this [power](power.md) is zero. For a [rigid body](rigid-body-dynamics-split.md), adding the translational and rotational contributions gives $\mathbf f_s\cdot\mathbf V_{\mathrm{CM}}+\boldsymbol\tau_{\mathrm{CM}}\cdot\boldsymbol\omega=\mathbf f_s\cdot\mathbf v_c$, where $\boldsymbol\tau_{\mathrm{CM}}$ is the contact [torque](torque.md) about the [center of mass](center-of-mass.md) and $\boldsymbol\omega$ its [angular velocity](angular-velocity.md). Counting only the first term omits the rotational contribution.

At a moving contact with zero [contact slip](contact-slip.md), the two material contact points share a [velocity](velocity.md) $\mathbf v_c$ that can be nonzero. For instance, a nonrotating block moving with an accelerating belt receives positive contact [power](power.md) $f_sU$ when the belt's rightward [velocity](velocity.md) $U$ and rightward [static friction](static-friction.md) $f_s$ are positive. The belt receives $-f_sU$ by [Newton's third law](newton-s-third-law.md). These contact contributions sum to zero in the ideal no-slip model, while the block's [kinetic energy](kinetic-energy.md) can increase. Zero [contact slip](contact-slip.md) and zero [work](work.md) on each body are different conditions.

**Table of contents**

- [Friction angle](friction-angle.md)
  - [Normal versus resultant force in a frictional pinch](normal-versus-resultant-force-in-a-frictional-pinch.md)
    - [No-lift threshold of a wedge pinch](no-lift-threshold-of-a-wedge-pinch.md)
- [Coefficient of static friction](coefficient-of-static-friction.md)
  - [Static friction on an inclined plane](static-friction-on-an-inclined-plane.md)
    - [Inclined-plane measurement of static friction](inclined-plane-measurement-of-static-friction.md)

## ↑ Ancestors (5)

1. [Force](force-split.md)
2. [Classical mechanics](classical-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Coefficient of static friction](coefficient-of-static-friction.md)
- [Constant-burn rocket with ground friction](constant-burn-rocket-with-ground-friction.md)
- [Constant-speed measurement of kinetic friction](constant-speed-measurement-of-kinetic-friction.md)
- [Friction](friction.md)
- [Friction angle](friction-angle.md)
- [Inclined plane](inclined-plane.md)
- [Kinetic friction](kinetic-friction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/3e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/12b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/9b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345/4/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1/section-a/a1/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/section-b/b8/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/section-a/a4/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/b7/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-c/10/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-b/6/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2019/2/solution.md)
- [Pulley coupled to a rolling disc](pulley-coupled-to-a-rolling-disc.md)
- [Rolling-cylinder loop contact threshold](rolling-cylinder-loop-contact-threshold.md)
- [Rolling-time factor on a straight incline](rolling-time-factor-on-a-straight-incline.md)
- [Sediment entrainment threshold](sediment-entrainment-threshold.md)
- [Shields parameter](shields-parameter.md)
- [Sliding acceleration on an inclined plane](sliding-acceleration-on-an-inclined-plane.md)
- [Slipping solid cylinder on an incline](slipping-solid-cylinder-on-an-incline.md)
- [Small oscillations inside a circular cylinder](small-oscillations-inside-a-circular-cylinder.md)
- [Spring-mounted rolling cylinder](spring-mounted-rolling-cylinder.md)
- [Static friction](static-friction.md)
- [Static friction on an inclined plane](static-friction-on-an-inclined-plane.md)
- [Vehicle rollover threshold](vehicle-rollover-threshold.md)
