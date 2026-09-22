<h1 id="a/2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The [water](../../../../../water.md) [mass conservation](../../../../../mass-conservation.md) equation inherited from the earlier model is $\epsilon h_t+(hu)_x=0$. It is essential: without it the printed displayed equations are not closed. Take the slow bed branch $\epsilon=0$, and perturb the uniform state by $h=1+\hat h e^{\lambda t+ikx}$, $u=1+Ue^{\lambda t+ikx}$, $c=1+Ce^{\lambda t+ikx}$, $s=Se^{\lambda t+ikx}$ and $\eta=1+\hat\eta e^{\lambda t+ikx}$. For $k\ne0$, [mass conservation](../../../../../mass-conservation.md) gives $\hat h=-U$ and $\hat\eta=S-U$.

Put $m=E^{*\prime}(1)+1$; the extra $1$ comes from linearizing $c/u$. The linearized [momentum](../../../../../momentum-split.md) and suspended-sediment equations are

$$
[3\delta+ik(F^2-1)]U=-ikS,\qquad (1+ik)C=mU,\qquad \lambda S=-mU+C.
$$

Eliminating $U,C$ gives the [dispersion relation](../../../../../dispersion-relation-split.md)

$$
\boxed{\lambda=-\frac{m k^2}{(1+ik)[3\delta+ik(F^2-1)]}.}
$$

Away from $F=1$, for fixed nonzero $k$ and negligible $\delta$,

$$
\operatorname{Re}\lambda=\frac{m k^2}{(F^2-1)(1+k^2)},\qquad \frac{\hat\eta}{S}=\frac{F^2}{F^2-1}.
$$

Thus growth requires $m/(F^2-1)>0$. For $F>1$, any $E^{*\prime}(1)>-1$ gives an unstable branch; for $F<1$ growth would require $E^{*\prime}(1)<-1$. A physically increasing erosion [function](../../../../../function-split.md) therefore gives the supercritical instability in this simplified model, rather than proving growth of ordinary subcritical dunes. Retaining drag gives

$$
\operatorname{Re}\lambda=\frac{m k^2[k^2(F^2-1)-3\delta]}{|(1+ik)[3\delta+ik(F^2-1)]|^2},
$$

which shows its stabilizing correction and the need to reconsider the limit near critical flow.

The negative bed-to-surface ratio for [subcritical flow](../../../../../subcritical-flow.md) means bed crests lie beneath surface troughs: the [dune](../../../../../dune.md) phase relation. Its positive sign for [supercritical flow](../../../../../supercritical-flow.md) gives aligned crests: an [antidune](../../../../../antidune.md). In the unstable supercritical case the imaginary part gives upstream migration, since $-\operatorname{Im}\lambda/k=-m/[(F^2-1)(1+k^2)]$. The figure shows these two phase relations. They identify the bedforms but do not by themselves establish growth. The qualitative limitation of the suspended-sediment mechanism is also discussed in the official [Mathematical Geoscience notes, pages 41–42](https://people.maths.ox.ac.uk/hewitt/publications/C5_11_notes.pdf).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
