<h1 id="a/2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At the retained order define $K=1+\tau r(I-S)$. Neglecting terms of order $a\tau$ in the incidence correction gives

$$
\dot I=rISK-aI,\qquad \dot S=-rISK.
$$

Dividing and expanding consistently,

$$
\frac{dI}{dS}=-1+\frac{a}{rSK}
=-1+\frac{a}{rS}+O(a\tau,\tau^2).
$$

Thus the [susceptible](../../../../../../susceptible-individual.md) count $S_*$ at the first threshold crossing obeys the same retained-order equation as before:

$$
I_*+S_*-\frac ar\log S_*=I_0+S_0-\frac ar\log S_0.
$$

It is important to distinguish completed case transfers at [quarantine](../../../../../../quarantine.md) from all [infections](../../../../../../infection.md) already initiated. Let the [quarantine](../../../../../../quarantine.md) time be $T$. Isolation prevents exposures after $T$, but animals exposed during $(T-\tau,T)$ still finish their [incubation period](../../../../../../incubation-period.md) during $(T,T+\tau)$. Their number, in the printed bookkeeping, is

$$
E_* =\int_{T-\tau}^{T}rI(s)S(s)\,ds
=\tau rI_*S_*+O(\tau^2).
$$

The [infection cases](../../../../../../infection-case.md) transferred by time $T$ among the initial $S$ class number $S_0-S_*$. Adding those pending [infection cases](../../../../../../infection-case.md) gives the eventual number who catch the [infectious disease](../../../../../../infectious-disease.md):

$$
\boxed{S_0-S_*+\tau rI_*S_*\quad\text{to the retained order}.}
$$

This adds only [infections](../../../../../../infection.md) caused by exposures before isolation; it does not allow secondary transmission after [quarantine](../../../../../../quarantine.md). If one asks instead only for the transfers completed by the instant of [quarantine](../../../../../../quarantine.md), the answer is $S_0-S_*$. The distinction is necessary because the model keeps incubating animals in its $S$ [compartment](../../../../../../compartment.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
