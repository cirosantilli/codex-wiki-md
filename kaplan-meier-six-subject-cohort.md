<h1 id="kaplan-meier-six-subject-cohort">Kaplan–Meier six-subject cohort</h1>

↑ **Parent:** [Kaplan–Meier estimator](kaplan-meier-estimator.md)

Consider six subjects observed from time zero. Recorded [survival data](survival-data.md) are $A:(1,1)$, $B:(2,0)$, $C:(3,1)$, $D:(3,1)$, $E:(3,0)$, and $F:(5,0)$, with each pair giving $(Y,\delta)$ in years. Thus $A,C,D$ have observed events, while $B,E,F$ are [right-censored](right-censoring.md). The letters label subjects, not treatment groups. Here are all exit times, including rows without events:

<a id="table-risk-sets-and-exact-kaplan-meier-steps-for-the-six-subject-cohort"></a>
| Time $t$ (years) | [Risk set](risk-set.md) just before $t$ | At risk $n$ | Events $d$ | [Right censoring](right-censoring.md) count $c$ | Survival factor $1-d/n$ | [Kaplan–Meier estimator](kaplan-meier-estimator.md) $\widehat S(t)$ |
| --- | --- | --- | --- | --- | --- | --- |
| $1$ | $A,B,C,D,E,F$ | $6$ | $1$ | $0$ | $5/6$ | $5/6$ |
| $2$ | $B,C,D,E,F$ | $5$ | $0$ | $1$ | $1$ | $5/6$ |
| $3$ | $C,D,E,F$ | $4$ | $2$ | $1$ | $1/2$ | $5/12$ |
| $5$ | $F$ | $1$ | $0$ | $1$ | $1$ | $5/12$ |

At year one, $\widehat S(1)=1(1-1/6)=5/6$. Removing $B$ at year two leaves the [Kaplan–Meier estimator](kaplan-meier-estimator.md) unchanged. Immediately before year three, $C,D,E,F$ are still in the [risk set](risk-set.md): the two events give $\widehat S(3)=(5/6)(1-2/4)=5/12\approx0.416667$. Only afterwards do $C,D,E$ leave, leaving $F$ alone. Removing $E$ before counting the tied events would incorrectly use $n=3$ and give $(5/6)(1-2/3)=5/18$. The event-first convention is part of the recorded-time interpretation; coarsely rounded timestamps do not reveal a hidden ordering within that time bin.

The exact [Kaplan–Meier estimator](kaplan-meier-estimator.md) is $1$ on $[0,1)$, $5/6$ on $[1,3)$, and $5/12$ on $[3,5]$. The three [right censoring](right-censoring.md) ticks are $(2,5/6)$, $(3,5/12)$, and $(5,5/12)$; at a shared event time the tick is on the post-event step. Beyond year five the [risk set](risk-set.md) is empty, so the horizontal endpoint does not determine later survival. The [Kaplan–Meier median survival time](kaplan-meier-median-survival-time.md) is three years, since this is the first step at or below $1/2$.

Now separate the tied events by changing only $D$'s recorded event time from year three to year four. At year three the [risk set](risk-set.md) still has four subjects, but $d=1$, so $\widehat S(3)=(5/6)(3/4)=5/8$. After the event and $E$'s [right censoring](right-censoring.md), only $D,F$ remain. At year four $n=2,d=1$, giving $\widehat S(4)=(5/8)(1/2)=5/16=0.3125$. The intervening [right censoring](right-censoring.md) prevents the factors from telescoping to the original tied-event factor. If $E$ instead remained observed past year four, the factors would be $(3/4)(2/3)=1/2$, giving the original $5/12$ after both events. This is [Kaplan–Meier telescoping across a censor-free interval](kaplan-meier-telescoping-across-a-censor-free-interval.md) in numbers.

Incorrectly counting every [right-censored](right-censoring.md) exit as an event estimates the distribution of observation-ending times $Y$, rather than [survival times](survival-time.md) $T$. For the original tied cohort, the spurious curve is $5/6$ at year one, $(5/6)(4/5)=2/3$ at year two, $(2/3)(1-3/4)=1/6$ at year three, and zero at year five. That zero asserts a failure for $F$, whose only known information is $T_F>5$.

<a id="image-six-observed-histories-and-the-effect-of-ties-and-right-censoring-on-kaplan-meier-steps"></a>
![](kaplan-meier-censored-cohort.png)

**[Figure 2](#image-six-observed-histories-and-the-effect-of-ties-and-right-censoring-on-kaplan-meier-steps). Six observed histories and the effect of ties and right censoring on Kaplan–Meier steps**.

The computation uses the [risk set](risk-set.md) and event-before-[censoring](censoring-statistics.md) convention in [Lu Tian's STAT331 notes, Unit 3, pages 2–6](https://web.stanford.edu/~lutian/coursepdf/STAT331unit3.pdf); this six-subject example supplies its own exact counts.

## ↑ Ancestors (6)

1. [Kaplan–Meier estimator](kaplan-meier-estimator.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Right censoring](right-censoring.md)
