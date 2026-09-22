# Pairwise independence does not imply joint independence

↑ **Parent:** [Pairwise independent random variables](pairwise-independent-random-variables.md)

Let $X,Y$ be [independent](independent-random-variables.md) fair [bits](bit.md), and let $Z=X\mathbin\oplus Y$ be their [exclusive or](exclusive-or.md): $Z=1$ precisely when $X\ne Y$. The four possible triples are $000,011,101,110$, each with [probability](probability.md) $1/4$. Each coordinate is a fair [bit](bit.md). Writing out all eight patterns gives

$$
\begin{array}{c|cccccccc}
(x,y,z)&000&001&010&011&100&101&110&111\\\hline
p_{X,Y,Z}(x,y,z)&1/4&0&0&1/4&0&1/4&1/4&0\\
p_X(x)p_Y(y)p_Z(z)&1/8&1/8&1/8&1/8&1/8&1/8&1/8&1/8
\end{array}
$$

Every pair has all four cells $00,01,10,11$ with [probability](probability.md) $1/4$:

$$
J_{X,Y}=J_{X,Z}=J_{Y,Z}
=\begin{pmatrix}1/4&1/4\\1/4&1/4\end{pmatrix}.
$$

For $(X,Z)$, the four allowed triples project to $00,01,11,10$; for $(Y,Z)$ they project to $00,11,01,10$. Each projection lists each pair exactly once, proving pairwise independence. But $\mathbb P(X=0,Y=0,Z=0)=1/4$ differs from the product $1/8$, so the three are not [independent random variables](independent-random-variables.md). Indeed, any two determine the third. A single coordinate reveals nothing about another, while two coordinates together reveal it completely.

<a id="image-the-xor-example-hides-joint-dependence-from-every-pairwise-probability-table"></a>
![](pairwise-versus-joint-independence.png)

**[Figure 3](#image-the-xor-example-hides-joint-dependence-from-every-pairwise-probability-table). The XOR example hides joint dependence from every pairwise probability table**. The bars show all eight triple patterns against the $1/8$ reference for three [independent](independent-random-variables.md) fair [bits](bit.md). Below, all three pairwise [joint probability mass functions](joint-probability-mass-function.md) have four equal cells of $1/4$.

The [exclusive or](exclusive-or.md) example is the complementary-bit version of the two-toss exercise in [Grinstead and Snell, Introduction to Probability, section 4.1, exercise 7, printed page 151](https://chance.dartmouth.edu/teaching_aids/books_articles/probability_book/Chapter4.pdf). It is a compact reason to check the full product rule whenever a calculation uses three-way or higher [events](event.md).

## ↑ Ancestors (8)

1. [Pairwise independent random variables](pairwise-independent-random-variables.md)
2. [Independent random variables](independent-random-variables.md)
3. [Random variable](random-variable-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Conditioning can destroy independence](conditioning-can-destroy-independence.md)
- [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)
- [Parity construction of pairwise independent bits](parity-construction-of-pairwise-independent-bits.md)
- [Return period](return-period.md)
