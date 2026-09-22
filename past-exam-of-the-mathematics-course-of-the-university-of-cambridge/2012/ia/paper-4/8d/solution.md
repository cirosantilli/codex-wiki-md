<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

First apply the [Cantor theorem](../../../../../cantor-s-theorem.md) by diagonalization. If an [injection](../../../../../injective-function.md) $j:\mathcal P(\mathbb R)\to\mathbb R$ existed, it would define a [surjection](../../../../../surjective-function.md) $h:\mathbb R\to\mathcal P(\mathbb R)$ by the unique inverse value on $j$'s image, and by $h(x)=\varnothing$ elsewhere. The [set](../../../../../set-split.md) $D=\{x\in\mathbb R:x\notin h(x)\}$ cannot equal $h(a)$ for any $a$, since $a\in D$ would be equivalent to $a\notin D$. This contradicts surjectivity. **There is no injection from the power [set](../../../../../set-split.md) of the real line into the real line.**

For the opposite type of encoding, let $b(x)=\tfrac12+\pi^{-1}\arctan x$, an injective [map](../../../../../function-class.md) from $\mathbb R$ to $(0,1)$. Give $b(x)$ its canonical [binary expansion](../../../../../binary-expansion.md), choosing the terminating expansion with trailing zeros whenever two expansions exist. If the binary digits of $b(x),b(y)$ are $a_j,b_j$, define a [real-number pairing by separated digits](../../../../../real-number-pairing-by-separated-digits.md):

$$
H(x,y)=\sum_{j\geq1}\left(\frac{2a_j}{3^{2j-1}}+\frac{2b_j}{3^{2j}}\right).
$$

This uses ternary digits only $0,2$, alternating the two input digit sequences. If two outputs first differ at ternary position $k$, that difference has magnitude $2\cdot3^{-k}$, while every later digit together contributes at most $\sum_{j>k}2\cdot3^{-j}=3^{-k}$. Their outputs therefore differ. The digits recover both binary sequences, hence both inputs. Neither output endpoint $0$ nor $1$ occurs because the input numbers lie strictly between zero and one. Thus **$H$ is an injection from $\mathbb R^2$ into $(0,1)\subset\mathbb R$**. The ternary construction avoids an unjustified decimal-interleaving argument at ambiguous expansions.

For a [finite modification of the identity on the real line](../../../../../finite-modification-of-the-identity-on-the-real-line.md), let $D_f=\{x:f(x)\ne x\}$ have size $n$, and sort it uniquely as $x_1<\cdots<x_n$. Its finite record is $(x_1,f(x_1),\ldots,x_n,f(x_n))$. It determines $f$ completely, with the identity used outside the recorded points. Repeatedly applying the pairing $H$ gives an [injection](../../../../../injective-function.md) $H_k:\mathbb R^k\to(0,1)$ for every positive finite $k$: take $H_1=b$ and $H_k(t_1,\ldots,t_k)=H(t_1,H_{k-1}(t_2,\ldots,t_k))$. Encode $f$ by

$$
J(f)=\begin{cases}1/2,&n=0,\\ n+H_{2n}(x_1,f(x_1),\ldots,x_n,f(x_n)),&n\geq1.\end{cases}
$$

Different lengths occupy disjoint intervals $(n,n+1)$, and within a fixed length the record is recoverable. Hence

$$
\boxed{\text{There is an injection }X\to\mathbb R.}
$$

Indeed the cardinality is exactly that of $\mathbb R$: the [functions](../../../../../function-split.md) that alter only $0$, assigning it an arbitrary real value, give an injection in the other direction, and the [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) applies.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
