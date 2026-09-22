# Conditional mutual information

↑ **Parent:** [Mutual information](mutual-information.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_mutual_information)

For finite [discrete random variables](discrete-random-variable.md), conditional mutual information measures the average reduction in uncertainty about $X$ from observing $Y$, when $Z$ is already known. With base-two [logarithms](logarithm.md), it is measured in [bits](bit.md):

$$
I(X;Y\mid Z)=H(X\mid Z)-H(X\mid Y,Z)
=H(X\mid Z)+H(Y\mid Z)-H(X,Y\mid Z).
$$

The second expression follows from the [chain rule for conditional entropy](chain-rule-for-conditional-entropy.md) and makes the symmetry in $X,Y$ visible. Equivalently, compute the [mutual information](mutual-information.md) separately in each conditional [probability distribution](probability-distribution-split.md) and then average:

$$
\begin{aligned}
I(X;Y\mid Z)
&=\sum_{z:p_Z(z)>0}p_Z(z)I(X;Y\mid Z=z)\\
&=\sum_{z:p_Z(z)>0}p_Z(z)
D\!\left(p_{X,Y\mid z}\,\middle\Vert\,p_{X\mid z}p_{Y\mid z}\right)\\
&=\sum_{x,y,z:p(x,y,z)>0}p(x,y,z)
\log_2\frac{p(x,y\mid z)}{p(x\mid z)p(y\mid z)}.
\end{aligned}
$$

Here $D$ is the [Kullback-Leibler divergence](kullback-leibler-divergence.md), also computed with base-two [logarithms](logarithm.md); zero-probability terms contribute zero. The [Gibbs inequality](gibbs-inequality.md) gives $I(X;Y\mid Z)\geq0$, with equality exactly when $X$ and $Y$ have [conditional independence](conditional-independence.md) given $Z$: the conditional joint [probability mass function](probability-mass-function.md) factors for every $z$ of positive [probability](probability.md).[Definition 2.4 and Theorem 2.5(1)](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-2-information-measures-mutual-information.md)

For a fully computed example, take [independent random variables](independent-random-variables.md) $X,Y$ that are fair [bits](bit.md), and let $Z=X\oplus Y$, where $\oplus$ is [exclusive or](exclusive-or.md). The complete joint [probability distribution](probability-distribution-split.md) has only these four positive entries:

<a id="table-joint-probabilities-for-two-independent-fair-bits-and-their-exclusive-or"></a>
| $X$ | $Y$ | $Z=X\oplus Y$ | $p(x,y,z)$ |
| --- | --- | --- | --- |
| $0$ | $0$ | $0$ | $1/4$ |
| $0$ | $1$ | $1$ | $1/4$ |
| $1$ | $0$ | $1$ | $1/4$ |
| $1$ | $1$ | $0$ | $1/4$ |

Every pair $(x,y)$ has [probability](probability.md) $1/4=p_X(x)p_Y(y)$, so $I(X;Y)=4(1/4)\log_2 1=0$. But $p_Z(0)=p_Z(1)=1/2$. Given $Z=0$, the pairs $(0,0),(1,1)$ each have conditional [probability](probability.md) $1/2$, while both conditional marginals are fair. Thus

$$
I(X;Y\mid Z=0)
=\frac12\log_2\frac{1/2}{(1/2)(1/2)}
+\frac12\log_2\frac{1/2}{(1/2)(1/2)}=1.
$$

Given $Z=1$, the pairs $(0,1),(1,0)$ give the same calculation. Therefore

$$
I(X;Y\mid Z)=\frac12\cdot1+\frac12\cdot1=1.
$$

The [conditional entropy](conditional-entropy.md) calculation tells the same story: $H(X\mid Z)=1$ because either value of $Z$ leaves $X$ fair, whereas $H(X\mid Y,Z)=0$ because $X=Y\oplus Z$. Learning the [exclusive or](exclusive-or.md) does not reveal either [bit](bit.md) alone; it reveals whether they agree, so learning one then determines the other.

<a id="image-conditioning-on-the-exclusive-or-reveals-one-bit-of-dependence-between-independent-fair-bits"></a>
![](conditional-information-xor.png)

**[Figure 7](#image-conditioning-on-the-exclusive-or-reveals-one-bit-of-dependence-between-independent-fair-bits). Conditioning on the exclusive or reveals one bit of dependence between independent fair bits**.

This example distinguishes [conditional independence](conditional-independence.md) from ordinary [independence](independent-random-variables.md). It also disproves the claim that conditioning always reduces [mutual information](mutual-information.md), despite [conditioning reduces entropy](conditioning-reduces-entropy.md). There is no general ordering between $I(X;Y\mid Z)$ and $I(X;Y)$: the example above increases it from zero to one, while taking $Y=X$ and $Z=X$ for a fair [bit](bit.md) decreases it from one to zero. The [chain rule for mutual information](chain-rule-for-mutual-information.md) explains why both are possible.[Theorem 2.5](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-2-information-measures-mutual-information.md)

[Conditional mutual information](conditional-mutual-information.md) is useful for asking whether an additional observation tells us anything after information already available has been accounted for. Its zero case expresses [conditional independence](conditional-independence.md) exactly; in a [Markov chain](markov-chain-split.md), this is the step that turns the [chain rule for mutual information](chain-rule-for-mutual-information.md) into the [data processing inequality](data-processing-inequality.md).

## ↑ Ancestors (6)

1. [Mutual information](mutual-information.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Chain rule for mutual information](chain-rule-for-mutual-information.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Data processing inequality](data-processing-inequality.md)
- [Entropy submodularity](entropy-submodularity.md)
- [Equality in data processing inequality](equality-in-data-processing-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/1/a/solution.md)
