# Entrainment of circadian rhythm

↑ **Parent:** [Circadian rhythm](circadian-rhythm.md)

[Entrainment of circadian rhythm](entrainment-of-circadian-rhythm.md) synchronizes a [circadian clock](circadian-clock.md) to a repeating cue, a [zeitgeber](zeitgeber.md). One-to-one [entrainment of circadian rhythm](entrainment-of-circadian-rhythm.md) gives one cycle per environmental cycle with a stable relative [circadian phase](circadian-phase.md).[pp. 86–87, synchronization to external cues; p. 92, Entrainment and Zeitgeber](overview-of-circadian-rhythms-by-martha-hotz-vitaterna-and-others.md) The stable relation need not put an activity onset exactly at lights-off: a constant offset also expresses [phase locking](phase-locking.md).

For an original local model, let $x_n$ be the activity-onset offset from lights-off on environmental cycle $n$, with a negative value meaning an earlier onset. Choose an intrinsic [period](period-of-a-function.md) $\tau=23.5\,\mathrm h$ and environmental [period](period-of-a-function.md) $T=24\,\mathrm h$. Let $D(x)$ be a stipulated daily delay, measured in hours; positive $D$ moves the next onset later. The [recurrence relation](recurrence-relation.md) is

$$
x_{n+1}=x_n+(\tau-T)+D(x_n).
$$

A fixed phase relationship $x_*$ requires $D(x_*)=T-\tau$: here a half-hour delay balances the half-hour intrinsic advance each cycle. This equality alone describes balance; restoration after a small disturbance also requires [fixed point stability for an iteration](fixed-point-stability-for-an-iteration.md).

Choose the illustrative local law $D(x)=0.5\,\mathrm h-0.4x$. Then

$$
x_{n+1}=0.6x_n,\qquad x_* =0,\qquad x_n=-3(0.6)^n\,\mathrm h
$$

for the chosen starting offset $x_0=-3\,\mathrm h$. The error shrinks by a factor of $0.6$ each cycle, proving [fixed point stability for an iteration](fixed-point-stability-for-an-iteration.md) in this model. After five cycles $x_5=-0.23328\,\mathrm h$, about fourteen minutes early. At the [fixed point](fixed-point.md), the imposed delay is $0.5\,\mathrm h$ and the corrected onset interval is $\tau+D(x_*)=24\,\mathrm h$, although the uncoupled [period](period-of-a-function.md) remains $23.5\,\mathrm h$.

<a id="image-circadian-entrainment-phase-correction"></a>
![](circadian-entrainment-phase-correction.png)

**[Figure 5](#image-circadian-entrainment-phase-correction). Daily phase correction restores a stable relation in an idealized entrainment of circadian rhythm model**. Original conceptual [circadian phase](circadian-phase.md) traces from the stated [recurrence relation](recurrence-relation.md). With the stipulated delay law, the offset approaches zero and the delay approaches half an hour. With no correction, the offset drifts earlier. The coefficient $0.4$ and starting offset are selected for explanation, not measured biological parameters. Lines join discrete cycle values.

The uncorrected comparison has $D=0$ and $x_n=-3\,\mathrm h+n(\tau-T)$, so after five cycles it is $5.5$ hours early. The two traces separate ongoing timekeeping from adjustment to a [zeitgeber](zeitgeber.md). The chosen linear delay law is only a local teaching construction: it is not a measured response to light, does not account for wrapping of [circadian phase](circadian-phase.md), and does not predict an organism's entrainment range. Nor does it include [masking of circadian rhythm](masking-of-circadian-rhythm.md). In a real study, tracking several cycles after removal of the cue or after a timed perturbation supplies information that a single activity value under illumination cannot provide.

**Table of contents**

- [Zeitgeber](zeitgeber.md)

## ↑ Ancestors (4)

1. [Circadian rhythm](circadian-rhythm.md)
2. [Physiology](physiology-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Circadian rhythm](circadian-rhythm.md)
- [Entrainment of circadian rhythm](entrainment-of-circadian-rhythm.md)
- [Free-running circadian rhythm](free-running-circadian-rhythm.md)
- [Solution](past-exam-of-the-plant-sciences-course-of-the-university-of-cambridge/2024/paper-plm1/3/solution.md)
