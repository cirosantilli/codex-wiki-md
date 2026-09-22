# An observation can increase entropy

↑ **Parent:** [Conditioning reduces entropy](conditioning-reduces-entropy.md)

Consider a binary state $X$ and a report $Y$ with the following [joint probability mass function](joint-probability-mass-function.md):

$$
\begin{array}{c|cc|c}
&Y=0&Y=1&p_X(x)\\\hline
X=0&4/5&1/10&9/10\\
X=1&0&1/10&1/10\\\hline
p_Y(y)&4/5&1/5&1
\end{array}
$$

Before the report, $X=0$ is strongly favored: its [information entropy](information-entropy-split.md) is $H(X)=h_2(1/10)\approx0.468996$ [bits](bit.md), where $h_2$ is [binary entropy](binary-entropy.md). A report $Y=1$ makes the two states equally likely, so $H(X\mid Y=1)=1$ [bit](bit.md), strictly larger than before. This report occurs with [probability](probability.md) $1/5$. The more common report $Y=0$ determines $X=0$, giving $H(X\mid Y=0)=0$. Therefore the averaged [conditional entropy](conditional-entropy.md) is

$$
H(X\mid Y)=\frac45\cdot0+\frac15\cdot1=\frac15<h_2(1/10)=H(X).
$$

The resulting [mutual information](mutual-information.md) is $I(X;Y)=h_2(1/10)-1/5\approx0.268996$ [bits](bit.md). The rare report increases uncertainty about the state; that increase does not make the report useless. Together the reports remove uncertainty on average. These are stipulated [probabilities](probability.md) in an exact model, not measured frequencies.

<a id="image-a-rare-report-raises-entropy-although-the-weighted-average-falls"></a>
![](conditioning-entropy-outcome-counterexample.png)

**[Figure 2](#image-a-rare-report-raises-entropy-although-the-weighted-average-falls). A rare report raises entropy although the weighted average falls**.

## ↑ Ancestors (7)

1. [Conditioning reduces entropy](conditioning-reduces-entropy.md)
2. [Conditional entropy](conditional-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
