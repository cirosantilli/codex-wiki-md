# Chain rule for mutual information

↑ **Parent:** [Mutual information](mutual-information.md)

For finite [discrete random variables](discrete-random-variable.md), the [mutual information](mutual-information.md) supplied by two observations equals the information supplied by the first plus the additional [conditional mutual information](conditional-mutual-information.md) supplied by the second:

$$
\begin{aligned}
I(X;Y,Z)&=I(X;Y)+I(X;Z\mid Y)\\
&=I(X;Z)+I(X;Y\mid Z).
\end{aligned}
$$

The order changes the individual contributions but leaves the total unchanged.[Stanford EE376A/STATS376A, Lecture 3, Definition 7 and equations (48)–(51)](https://web.stanford.edu/class/ee376a/files/lecture_3.pdf) To prove the first identity, add and subtract the intermediate [conditional entropy](conditional-entropy.md):

$$
\begin{aligned}
I(X;Y,Z)&=H(X)-H(X\mid Y,Z)\\
&=\bigl[H(X)-H(X\mid Y)\bigr]
+\bigl[H(X\mid Y)-H(X\mid Y,Z)\bigr].
\end{aligned}
$$

With base-two [logarithms](logarithm.md), all contributions are in [bits](bit.md). Repeatedly inserting intermediate [conditional entropies](conditional-entropy.md) makes them cancel, as in a [telescoping series](telescoping-series.md), and gives the rule for any finite list of observations:

$$
I(X;Y_1,\ldots,Y_n)=\sum_{j=1}^{n}I(X;Y_j\mid Y_1,\ldots,Y_{j-1}),
$$

where the $j=1$ term is $I(X;Y_1)$. The same calculation with $W$ already known gives $I(X;Y,Z\mid W)=I(X;Y\mid W)+I(X;Z\mid Y,W)$.

For the fair-[bit](bit.md) [exclusive or](exclusive-or.md) example in [conditional mutual information](conditional-mutual-information.md), observing $Y$ alone tells nothing about $X$, but observing $Z$ after $Y$ tells everything:

$$
I(X;Y,Z)=I(X;Y)+I(X;Z\mid Y)=0+(1-0)=1.
$$

Here $H(X\mid Y)=1$ by [independence](independent-random-variables.md) and $H(X\mid Y,Z)=0$ because $X=Y\oplus Z$. In the reverse order, $H(X\mid Z)=1$, so $I(X;Z)=0$ and $I(X;Y\mid Z)=1$: the two observations are individually uninformative but jointly reveal one [bit](bit.md). Simply adding their separate [mutual informations](mutual-information.md) would miss all of it.

The chain rule is useful for measuring the value of each new observation without double counting information already supplied. It also guarantees $I(X;Y,Z)\geq I(X;Y)$ by nonnegativity of [conditional mutual information](conditional-mutual-information.md). Keeping $Y$ and adding $Z$ can help, even though discarding $Y$ and retaining only a processed $Z$ is constrained by the [data processing inequality](data-processing-inequality.md). Equating the two observation orders gives the precise identity

$$
I(X;Y\mid Z)-I(X;Y)=I(X;Z\mid Y)-I(X;Z),
$$

which explains why there is no general rule that conditioning decreases [mutual information](mutual-information.md).

## ↑ Ancestors (6)

1. [Mutual information](mutual-information.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Conditional mutual information](conditional-mutual-information.md)
- [Data processing inequality](data-processing-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/11i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/1/a/solution.md)
