<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the 2017 calendar window to be $[1,13]$ on the supplied month scale. Intersecting each follow-up interval with this window and translating to time since diagnosis gives:

- patient 1: delayed entry at duration 10 and censoring at 22;
- patient 3: delayed entry at 8 and death at 15;
- patient 4: delayed entry at 4 and censoring at 7;
- patient 5: delayed entry at 2 and censoring at 14;
- patient 6: entry at 0 and censoring at 9;
- patient 7: entry at 0 and death at 6;
- patient 8: entry at 0 and censoring at 6;
- patient 9: entry at 0 and censoring at 4.

Patient 2 died before the period and patient 10 entered after it, so neither contributes. At duration 6, patients 4, 5, 6, 7, and 8 are at risk, giving factor $1-1/5=4/5$. At duration 15, patients 1 and 3 are at risk, giving factor $1-1/2=1/2$. Therefore the period [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) is

$$
\boxed{
\widehat S_{\mathrm{2017}}(t)=
\begin{cases}
1,&0\leq t<6,\\
4/5,&6\leq t<15,\\
2/5,&t\geq15.
\end{cases}}
$$

over the range supported by the period data.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
