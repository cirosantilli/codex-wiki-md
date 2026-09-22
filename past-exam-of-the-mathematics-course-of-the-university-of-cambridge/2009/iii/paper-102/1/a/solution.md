<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The examination used separately emailed files. For this question a public [Guerry data archive](https://github.com/friendly/Guerry) and its [CSV mirror](https://raw.githubusercontent.com/vincentarelbundock/Rdatasets/master/csv/HistData/Guerry.csv) permit a documented reconstruction: retain the 85 records with a recorded region and select the specified columns. All six printed records match exactly, and each of the five regions has 17 departments. The numerical results below refer to that reconstruction; the remaining rows cannot be checked against the unavailable emailed file.

Treat department identifiers as labels and region as a [categorical variable](../../../../../../categorical-variable.md). The following summaries show the scale and spread of the quantitative variables:

| Variable | Mean | Standard deviation | Median | Interquartile range | Range |
| --- | --- | --- | --- | --- | --- |
| CrimePers | 19960.94 | 7299.24 | 18785 | 14790–26221 | 5883–37014 |
| CrimeProp | 7881.34 | 3048.62 | 7624 | 5990–9190 | 1368–20235 |
| Literacy | 39.14 | 17.43 | 38 | 25–52 | 12–74 |
| Donations | 6723.32 | 4863.24 | 4964 | 3446–9242 | 1246–27830 |
| Wealth rank | 43.58 | 25.11 | 44 | 22–65 | 1–86 |

A larger population-per-crime value means a lower crime rate, and a smaller wealth rank means greater recorded wealth. Donations are markedly right-skewed, as the large gap between mean and median and the upper tail indicate; rank is an ordinal measure rather than a monetary difference. For the ratio analysed next, the median is $2.683$, the interquartile interval is $[1.829,3.515]$, and the range is $[0.643,10.194]$.

Regional median ratios are $2.763$ in C, $2.502$ in E, $3.979$ in N, $1.373$ in S, and $2.937$ in W. The regional [box plots](../../../../../../box-plot.md) and wealth-versus-log-ratio [scatter plot](../../../../../../scatter-plot.md) in the figure expose this geographical contrast and an inverse association with wealth rank. **North has the highest typical property-to-person crime ratio and South the lowest in the reconstructed data.** These summaries are descriptive departmental comparisons, not causal or individual-level conclusions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
