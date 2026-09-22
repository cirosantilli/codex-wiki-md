<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For six hours of operation at the maximum stated carbon-dioxide-equivalent flow, the daily input volume and untreated [radioactive activity](../../../../../radioactive-activity.md) inventory are

$$
V_d=Q(6)(3600)=7.992\times10^{-3} \mathrm{m^3},\qquad
D_{d,0}=a_0V_d=7.992\times10^{11} \mathrm{Bq}.
$$

For the three-hour guaranteed delay, every element of the incoming stream acquires the same [radioactive decay](../../../../../radioactive-decay.md) factor. The [radioactive activity](../../../../../radioactive-activity.md) released per operating day, attributing the delayed tail to its production day, is

$$
D_d=D_{d,0}e^{-\lambda(10800)}=\boxed{1.712\times10^9 \mathrm{Bq}}.
$$

Even on the conservative assumption of operation on all $365$ days,

$$
D_y=365D_d=\boxed{6.248\times10^{11} \mathrm{Bq\,yr^{-1}}},
$$

so the annual discharge is below the supplied $10^{12}$ Bq limit. For $250$ operating days it is $4.279\times10^{11}$ Bq. This sums [radioactive activity](../../../../../radioactive-activity.md) inventories discharged over the year; it does not credit [radioactive decay](../../../../../radioactive-decay.md) in the environment after release. It also retains the final delayed gas after production stops, rather than bypassing the retention system to empty it.

The residence-time qualification matters numerically. A single tank filled for six hours and released immediately, with [radioactive decay](../../../../../radioactive-decay.md) during filling but no later hold, would contain

$$
A_{\rm fill}(21600)=6.502\times10^{10} \mathrm{Bq}.
$$

Repeating that operation on $250$ days releases $1.625\times10^{13}$ Bq, **above the limit**. A well-mixed or fill-and-dump system therefore cannot inherit the plug-flow compliance result just because its nominal volume divided by flow equals the selected delay time. The total [nitrogen](../../../../../nitrogen.md) flow and any unretained radioactive carbon species must also be included in a real measured release account.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [2](../../2.md)
3. [Module NE4](../../../paper-ne4-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
