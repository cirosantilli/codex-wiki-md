# Chain decomposition of total correlation

↑ **Parent:** [Total correlation](total-correlation.md)

For finite [alphabets](alphabet.md), expanding [joint entropy](joint-entropy.md) with the [chain rule for information entropy](chain-rule-for-information-entropy.md) gives

$$
\operatorname{TC}(X_1,\ldots,X_n)
=\sum_{i=2}^n\bigl[H(X_i)-H(X_i\mid X_1,\ldots,X_{i-1})\bigr]
=\sum_{i=2}^n I(X_i;X_1,\ldots,X_{i-1}).
$$

Each term is [mutual information](mutual-information.md) with an entire preceding block, rather than necessarily with one preceding variable. Changing the order changes these individual terms but leaves their sum unchanged.

For the noiseless [parity constraint and total correlation](parity-constraint-and-total-correlation.md), $I(Y;X)=0$ and $I(Z;X,Y)=1$ [bit](bit.md). The conditional block term supplies exactly the dependence that the pairwise comparisons missed. For three identical copies of a fair [bit](bit.md), the two block terms are both one [bit](bit.md). Thus [total correlation](total-correlation.md) counts total departure from the product law, not merely the presence of a single irreducible multiway relation.

## ↑ Ancestors (6)

1. [Total correlation](total-correlation.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
