<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the [B2 root system](../../../../../b2-root-system.md) convention

$$
\alpha_1=\varepsilon_2,
\qquad
\alpha_2=\varepsilon_1-\varepsilon_2,
\qquad
\omega_1=\frac{\varepsilon_1+\varepsilon_2}{2},
\qquad
\omega_2=\varepsilon_1.
$$

Thus $V=L_{\omega_2}$ is the five-dimensional vector representation of the [Special orthogonal Lie algebra](../../../../../special-orthogonal-lie-algebra.md) $\mathfrak{so}_5$. Label its weight vertices

$$
A=\varepsilon_1,quad B=\varepsilon_2,quad C=0,quad D=-\varepsilon_2,quad E=-\varepsilon_1.
$$

The [crystal basis](../../../../../crystal-basis.md) is the colored chain

$$
A\xrightarrow{2}B\xrightarrow{1}C\xrightarrow{1}D\xrightarrow{2}E,
$$

because each [Kashiwara operator](../../../../../kashiwara-operator.md) $\widetilde f_i$ subtracts $\alpha_i$.

For the [tensor product of crystals](../../../../../tensor-product-of-crystals.md), write $XY$ for $X\otimes Y$. The complete colored-arrow graph is compactly specified by

$$
\begin{aligned}
\text{color }1:\quad&
AB\to AC\to AD,\quad BA\to CA\to DA,\quad
BB\to CB\to DB\to DC\to DD,\\
&BC\to CC\to CD,\quad BE\to CE\to DE,\quad EB\to EC\to ED;\\
\text{color }2:\quad&
AA\to BA\to BB,\quad AC\to BC,\quad AD\to BD\to BE,\\
&CA\to CB,\quad CD\to CE,\quad DA\to EA\to EB,\quad
DC\to EC,\quad DD\to ED\to EE.
\end{aligned}
$$

Its three connected highest-weight components start at $AA$, $AB$, and $AE$. Their vertex sets are

$$
\begin{aligned}
B(2\omega_2):\quad&AA,BA,BB,CA,CB,DA,DB,DC,DD,EA,EB,EC,ED,EE,\\
B(2\omega_1):\quad&AB,AC,AD,BC,BD,BE,CC,CD,CE,DE,\\
B(0):\quad&AE.
\end{aligned}
$$

Their highest weights and dimensions identify the ten-vertex component with the [exterior square](../../../../../exterior-square.md) and the other two with the [symmetric square](../../../../../symmetric-square.md). Therefore

$$
\bigwedge^2V\cong L_{2\omega_1},
\qquad
S^2V\cong L_{2\omega_2}\oplus L_0,
$$

of dimensions $10$ and $14+1$, respectively.

The module $L=L_{\omega_1}$ is the four-dimensional spin representation. Its weights are $(\pm\varepsilon_1\pm\varepsilon_2)/2$, and its crystal is

$$
\frac{\varepsilon_1+\varepsilon_2}{2}
\xrightarrow{1}
\frac{\varepsilon_1-\varepsilon_2}{2}
\xrightarrow{2}
\frac{-\varepsilon_1+\varepsilon_2}{2}
\xrightarrow{1}
\frac{-\varepsilon_1-\varepsilon_2}{2}.
$$

Every weight of $V$ lies in the [root lattice](../../../../../root-lattice.md), so every weight of every [tensor power](../../../../../tensor-power.md) $V^{\otimes n}$ also lies in that lattice. But $\omega_1=(\varepsilon_1+\varepsilon_2)/2$ represents the nonzero coset in the quotient of the [weight lattice](../../../../../weight-lattice.md) by the root lattice. Consequently no irreducible constituent of $V^{\otimes n}$ can have highest weight $\omega_1$, and $L$ never occurs.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
