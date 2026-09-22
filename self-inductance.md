# Self-inductance

↑ **Parent:** [Inductance](inductance.md)

[Self-inductance](self-inductance.md) is [inductance](inductance.md) associated with a coil's own [electric current](electric-current.md), rather than [magnetic flux](magnetic-flux.md) supplied by another coil. In the linear model, fixed geometry and magnetic response give constant $L$ in $\Lambda=LI$. With the turn orientations defined in [magnetic flux linkage](magnetic-flux-linkage.md), [Faraday's law of induction](faraday-s-law-of-induction.md) gives the self-induced [electromotive force](electromotive-force.md)

$$
\mathcal E_{\rm ind}=-\frac{d\Lambda}{dt}=-L\frac{dI}{dt}.
$$

The final equality requires constant $L$; if the geometry changes, use $-d\Lambda/dt$. The minus sign expresses [Lenz's law](lenz-s-law.md): the induced [electromotive force](electromotive-force.md) opposes the change in [electric current](electric-current.md). It does not always oppose the [electric current](electric-current.md) itself. When positive [electric current](electric-current.md) decreases, the induced [electromotive force](electromotive-force.md) acts in its direction. [OpenStax University Physics 2, §14.2: self-induced emf and its direction](https://openstax.org/books/university-physics-volume-2/pages/14-2-self-inductance-and-inductors).

For terminal sign bookkeeping, label the ideal [inductor](inductor.md)'s terminals $a,b$, choose positive [electric current](electric-current.md) entering $a$ and leaving $b$, and define $v_L$ as the terminal [electric potential difference](electric-potential-difference.md) drop from $a$ to $b$ in the lumped [electrical circuit](electrical-circuit.md) model. This passive convention gives

$$
v_L=+L\frac{dI}{dt}=-\mathcal E_{\rm ind}.
$$

Thus a coil with [self-inductance](self-inductance.md) $0.5\,\mathrm H$ and increasing [electric current](electric-current.md) $dI/dt=12\,\mathrm{A/s}$ has terminal drop $v_L=6\,\mathrm V$ and induced [electromotive force](electromotive-force.md) $\mathcal E_{\rm ind}=-6\,\mathrm V$. These signs describe the same process with different reference conventions. The [RL circuit](rl-circuit.md) uses the terminal-drop convention throughout.

A finite terminal [electric potential difference](electric-potential-difference.md) cannot make the [electric current](electric-current.md) of an ideal [inductor](inductor.md) with constant $L>0$ jump. Integrating its [differential equation](differential-equation-split.md) gives

$$
I(t_2)-I(t_1)=\frac1L\int_{t_1}^{t_2}v_L(t)\,dt.
$$

If $v_L$ stays bounded, the [integral](integral.md) tends to zero as the interval shrinks, ensuring [continuity](continuous-function.md) of [electric current](electric-current.md). A step in terminal [electric potential difference](electric-potential-difference.md) changes $dI/dt$ immediately, while [electric current](electric-current.md) remains continuous. At constant [electric current](electric-current.md), the self-induced [electromotive force](electromotive-force.md) is zero, although the [inductor](inductor.md)'s [magnetic energy](magnetic-energy.md) can remain nonzero.

**Table of contents**

- [Inductor](inductor.md)

## ↑ Ancestors (5)

1. [Inductance](inductance.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Electromotive force](electromotive-force.md)
- [Faraday's law of induction](faraday-s-law-of-induction.md)
- [Henry (unit)](henry-unit.md)
- [Inductance](inductance.md)
- [Inductor](inductor.md)
- [Lenz's law](lenz-s-law.md)
- [Lossless limit of magnetic loop braking](lossless-limit-of-magnetic-loop-braking.md)
- [Motional electromotive force](motional-electromotive-force.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2/17h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/7a/solution.md)
- [RL circuit](rl-circuit.md)
- [Self-inductance](self-inductance.md)
- [Solenoid inductance](solenoid-inductance.md)
- [Stored energy of a solenoid](stored-energy-of-a-solenoid.md)
