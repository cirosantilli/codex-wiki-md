<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $\oplus$ for [exclusive or](../../../../../exclusive-or.md) and regard all [bits](../../../../../bit.md) as elements of $\mathbb F_2$. For every public label $z\in\{0,1\}^m$, Alice computes the [indicator function](../../../../../indicator-function.md)

$$
u_z(x)=\mathbf1_{\{x=z\}},
$$

while Bob computes $v_z(y)=f(z,y)$ from the known [truth table](../../../../../truth-table.md). Exactly one of the $u_z(x)$ is one, so the [separated Boolean decomposition](../../../../../separated-boolean-decomposition.md) is

$$
f(x,y)=\bigoplus_{z\in\{0,1\}^m}u_z(x)v_z(y).
$$

For each $z$, they invoke an independent [PR box](../../../../../popescu-rohrlich-box.md) with respective input [bits](../../../../../bit.md) $u_z(x),v_z(y)$ and receive outputs $a_z,b_z$. These satisfy $a_z\oplus b_z=u_z(x)v_z(y)$. Alice forms $A=\bigoplus_z a_z$, and Bob forms $B=\bigoplus_z b_z$. Taking the [exclusive or](../../../../../exclusive-or.md) of all box constraints proves

$$
A\oplus B
=\bigoplus_z(a_z\oplus b_z)
=\bigoplus_z u_z(x)v_z(y)=f(x,y).
$$

Alice sends the single [bit](../../../../../bit.md) $A$. Bob combines it with his locally known $B$, obtaining

$$
\boxed{f(x,y)=A\oplus B,\qquad\text{one classical bit from Alice to Bob}.}
$$

This is [one-bit computation using Popescu–Rohrlich boxes](../../../../../one-bit-computation-using-popescu-rohrlich-boxes.md). It uses $2^m$ boxes; decomposing by Bob's input instead gives $2^n$, so the smaller truth-table factorization uses at most $2^{\min(m,n)}$. No efficiency bound on local calculation or box use is needed for the stated unlimited resource.

Each [PR box](../../../../../popescu-rohrlich-box.md) has uniform local output distributions regardless of the other party's input. Independent invocations therefore give Bob a uniform output string before the message, carrying no information about $x$. The useful correlation becomes accessible through Alice's final [bit](../../../../../bit.md); the construction respects the no-signalling property of the boxes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
