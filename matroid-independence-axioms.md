# Matroid independence axioms

↑ **Parent:** [Matroid](matroid.md)

Let $E$ be a [finite set](finite-set.md) and $\mathcal I\subseteq\mathcal P(E)$ a family of [subsets](subset.md), where $\mathcal P(E)$ is the [power set](power-set.md). The [matroid independence axioms](matroid-independence-axioms.md) are

$$
\begin{aligned}
&\varnothing\in\mathcal I,\\
&I\in\mathcal I,\ J\subseteq I\quad\Longrightarrow\quad J\in\mathcal I,\\
&I,J\in\mathcal I,\ |I|<|J|\quad\Longrightarrow\quad
\exists e\in J\setminus I:\ I\cup\{e\}\in\mathcal I.
\end{aligned}
$$

The second condition is heredity; the third is exchange, also called augmentation. The [set difference](set-difference.md) $J\setminus I$ matters: the new element must actually increase the [cardinality](cardinality.md) of $I$. Exchange adds one element without requiring any deletion from $I$. Nonemptiness together with heredity is equivalent to the first condition. [Michel X. Goemans, Matroid optimization, section 5.1, p. 1, axioms (I1) and (I2)](matroid-optimization-by-michel-goemans.md)

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Basis of a matroid](basis-of-a-matroid.md)
- [Graphic matroid](graphic-matroid.md)
- [Independence system](independence-system.md)
- [Matroid greedy algorithm](matroid-greedy-algorithm.md)
- [Matroid independence axioms](matroid-independence-axioms.md)
