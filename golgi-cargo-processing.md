# Golgi cargo processing

↑ **Parent:** [Golgi apparatus](golgi-apparatus.md)

[Golgi cargo processing](golgi-cargo-processing.md) includes [enzyme](enzyme-split.md)-mediated remodeling of attached [oligosaccharides](oligosaccharide.md). [Glycosylation](glycosylation.md) can involve addition of [sugars](sugar.md), while processing can also remove them. Different [Golgi apparatus](golgi-apparatus.md) regions have different processing [enzymes](enzyme-split.md); their [substrate](substrate-biochemistry.md) requirements constrain the order of possible [chemical reactions](chemical-reaction-split.md).[Molecular Biology of the Cell, 4th edition by Bruce Alberts and others; Oligosaccharide Chains Are Processed in the Golgi Apparatus; The Golgi Cisternae Are Organized as a Series of Processing Compartments, Figure 13-28](molecular-biology-of-the-cell-4th-edition-by-bruce-alberts-and-others/transport-from-the-er-through-the-golgi-apparatus.md)

An original model makes the importance of ordering explicit. Write a toy [carbohydrate](carbohydrate.md) chain as $XA$, read with its terminal symbol on the right. Define a trimming [function](function-split.md) $T$ that removes a terminal $A$, and an extension [function](function-split.md) $E$ that adds $B$ only when the terminal symbol is $X$. In every other case the corresponding [function](function-split.md) leaves the chain unchanged. Then

$$
XA\xrightarrow{T}X\xrightarrow{E}XB,\qquad XA\xrightarrow{E}XA\xrightarrow{T}X.
$$

In particular, $E(T(XA))=XB$ but $T(E(XA))=X$: the two [functions](function-split.md) do not commute. Each result follows by inspecting the terminal symbol before applying the stipulated rule. These symbols are artificial labels, rather than a natural [oligosaccharide](oligosaccharide.md) sequence or measured [enzyme](enzyme-split.md) pathway. The example explains why “two processing steps occurred” does not determine the product unless their order and [substrate](substrate-biochemistry.md) conditions are also specified. In the [Golgi apparatus](golgi-apparatus.md), spatial organization can help arrange successive opportunities for processing.

## ↑ Ancestors (5)

1. [Golgi apparatus](golgi-apparatus.md)
2. [Organelle](organelle.md)
3. [Biological cell](biological-cell-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Golgi cargo processing](golgi-cargo-processing.md)
- [Oligosaccharide](oligosaccharide.md)
