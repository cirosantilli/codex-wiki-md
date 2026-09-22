# Joint entropy

↑ **Parent:** [Information entropy](information-entropy.md)

[Joint entropy](joint-entropy.md) is the [information entropy](information-entropy.md) of an entire [random vector](random-vector.md), treating its coordinates together as one outcome. For [random variables](random-variable-split.md) with finite [alphabets](alphabet.md) and joint [probability mass function](probability-mass-function.md) $p$,

$$
H(X_1,\ldots,X_n)=-\sum_{x_1,\ldots,x_n:p(x_1,\ldots,x_n)>0}p(x_1,\ldots,x_n)\log_2 p(x_1,\ldots,x_n).
$$

It is measured in [bits](bit.md). The distinction from separate [information entropies](information-entropy.md) is whether shared uncertainty is counted once or repeatedly. Two copies of the same fair [bit](bit.md) have [joint entropy](joint-entropy.md) one [bit](bit.md), since only $00$ and $11$ can occur. Two [independent](independent-random-variables.md) fair [bits](bit.md) have [joint entropy](joint-entropy.md) two [bits](bit.md), since all four pairs are possible and equiprobable.

For a less symmetric example, assign [probabilities](probability.md) $1/2,1/4,1/4$ to $(X,Y)=(0,0),(1,0),(1,1)$ respectively. Then

$$
\boxed{H(X,Y)=\tfrac12\cdot1+\tfrac14\cdot2+\tfrac14\cdot2=\tfrac32\text{ bits}.}
$$

Here $X$ is fair, while $\mathbb P(Y=1)=1/4$. Thus $H(X)=1$ and $H(Y)=h_2(1/4)\approx0.811278$ [bits](bit.md), where $h_2$ is [binary entropy](binary-entropy.md). Adding the separate [information entropies](information-entropy.md) would give approximately $1.811278$ [bits](bit.md), overcounting by the [mutual information](mutual-information.md) $I(X;Y)\approx0.311278$ [bits](bit.md).

The [chain rule for information entropy](chain-rule-for-information-entropy.md) makes the shared information explicit:

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

In this example $Y$ is certain given $X=0$ and fair given $X=1$, so its average [conditional entropy](conditional-entropy.md) is $H(Y\mid X)=\tfrac12\cdot0+\tfrac12\cdot1=1/2$ [bit](bit.md). Sending the first coordinate changes how much uncertainty remains in the second. A [prefix code](prefix-code.md) with codewords `0`, `10`, `11` for the three possible pairs has average length $3/2$ [bits](bit.md), exactly the [joint entropy](joint-entropy.md) in this stipulated law.

For finite [alphabets](alphabet.md),

$$
\max_iH(X_i)\leq H(X_1,\ldots,X_n)\leq\sum_iH(X_i).
$$

The lower bound follows because knowing the full [random vector](random-vector.md) determines every coordinate; the upper bound follows from [conditioning reduces entropy](conditioning-reduces-entropy.md) in the [chain rule for information entropy](chain-rule-for-information-entropy.md). Equality in the upper bound means joint [independence](independent-random-variables.md). The difference from that upper bound is [total correlation](total-correlation.md), whose [noisy parity total correlation](noisy-parity-total-correlation.md) example shows why separate pairwise comparisons need not find all the dependence.

## ↑ Ancestors (6)

1. [Information entropy](information-entropy.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Chain decomposition of total correlation](chain-decomposition-of-total-correlation.md)
- [Historical source for total correlation](historical-source-for-total-correlation.md)
- [Joint entropy](joint-entropy.md)
- [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/2/solution.md)
- [Total correlation](total-correlation.md)
