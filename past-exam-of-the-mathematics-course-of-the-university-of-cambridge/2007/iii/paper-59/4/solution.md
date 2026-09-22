<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use $\oplus$ for addition modulo two, or [exclusive or](../../../../../exclusive-or.md). The key is to write the known [Boolean function](../../../../../boolean-function.md) as an XOR of products of locally computable bits. An explicit [separated Boolean decomposition](../../../../../separated-boolean-decomposition.md) avoids any need to assume a particular circuit for the function. For every possible Alice input $\xi\in\{0,1\}^m$, put

$$
u_\xi(x)=\mathbf1_{\{x=\xi\}},\qquad v_\xi(y)=f(\xi,y).
$$

Alice can compute the first bit from her actual input and the public label $\xi$; Bob can compute the second bit from his own input because $\xi$ and the full function are public. Exactly one of the indicators is one, namely the one with $\xi=x$. Hence

$$
\boxed{f(x,y)=\bigoplus_{\xi\in\{0,1\}^m}u_\xi(x)v_\xi(y).}
$$

For each label $\xi$, invoke one independent [Popescu–Rohrlich box](../../../../../popescu-rohrlich-box.md) with inputs $u_\xi(x)$ and $v_\xi(y)$. Denote its outputs by $a_\xi$ and $b_\xi$. By the given correlation, $a_\xi\oplus b_\xi=u_\xi v_\xi$. Alice locally forms $A=\bigoplus_\xi a_\xi$, and Bob locally forms $B=\bigoplus_\xi b_\xi$. Taking the XOR of all box constraints yields

$$
A\oplus B=\bigoplus_\xi(a_\xi\oplus b_\xi)=\bigoplus_\xi u_\xi(x)v_\xi(y)=f(x,y).
$$

Thus the protocol is

$$
\boxed{\text{Alice sends the single bit }A;\qquad\text{Bob outputs }A\oplus B=f(x,y).}
$$

**It succeeds exactly for every input and every allowed sequence of box outputs.** Randomness of the individual outputs introduces no error because each parity relation is exact. All box calls can be made before the message, with no extra classical communication. This proves [one-bit computation using Popescu–Rohrlich boxes](../../../../../one-bit-computation-using-popescu-rohrlich-boxes.md).

The truth-table construction uses $2^m$ [PR boxes](../../../../../popescu-rohrlich-box.md). If Bob's input is shorter, use the equally valid decomposition $f(x,y)=\bigoplus_{\eta\in\{0,1\}^n}f(x,\eta)\mathbf1_{\{y=\eta\}}$. Alice computes the first factor, Bob the indicator, and Alice still sends her output parity. Therefore at most $2^{\min(m,n)}$ boxes are enough. This is a bound on box use, not on local computational work; the [communication complexity](../../../../../communication-complexity.md) remains one bit.

Another standard route is the [algebraic normal form](../../../../../algebraic-normal-form.md) over the two-element field:

$$
f(x,y)=\bigoplus_{I\subseteq\{1,\ldots,m\},\ J\subseteq\{1,\ldots,n\}}c_{IJ}\left(\prod_{i\in I}x_i\right)\left(\prod_{j\in J}y_j\right),\qquad c_{IJ}\in\{0,1\}.
$$

The empty products are one. For completeness, this representation follows by induction on the number of bits from $f(z',z_d)=f(z',0)\oplus z_d[f(z',0)\oplus f(z',1)]$, which adds a new variable only to its corresponding coefficients. Each nonzero monomial supplies one local product to each party and can be evaluated in distributed parity form by one [PR box](../../../../../popescu-rohrlich-box.md). Terms depending on only one party can instead be included directly in that party's final parity; the constant may be assigned to either side. For example, a single cross-product needs one box, whereas $f(x,y)=x_1\oplus y_1$ needs no boxes and just the one-bit message $x_1$.

Finally, the scheme does not make the boxes themselves signalling devices. At any fixed box inputs, the two allowed output pairs give each party an individually uniform bit, independent of the distant input. Independence across box calls makes Bob's entire uncommunicated output string uniform, for any Alice input. Without $A$ he generally cannot identify the answer. The communicated parity combines with the nonlocal correlations to reveal it; it does not contradict the uniform local marginals of these [no-signalling boxes](../../../../../no-signalling-box.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
