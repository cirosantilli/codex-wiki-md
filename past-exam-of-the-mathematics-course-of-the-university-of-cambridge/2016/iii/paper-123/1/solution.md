<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the simple-root form of [Hensel lemma](../../../../../hensel-s-lemma.md): if $F\in\mathbb Z_p[T]$ and $t_0\in\mathbb Z_p$ satisfy $F(t_0)\equiv0\pmod p$ and $F'(t_0)\not\equiv0\pmod p$, there is a unique $t\in\mathbb Z_p$ with $F(t)=0$ and $t\equiv t_0\pmod p$. More generally the same assertion holds over a complete [discrete valuation ring](../../../../../discrete-valuation-ring.md), with its [maximal ideal](../../../../../maximal-ideal.md) in place of $(p)$.

Every nonzero [3-adic number](../../../../../3-adic-number.md) has a unique expression

$$
x=3^k\epsilon u,\qquad k\in\mathbb Z,\quad\epsilon\in\{1,-1\},\quad u\in U_1:=1+3\mathbb Z_3.
$$

Indeed its normalized [P-adic valuation](../../../../../p-adic-valuation.md) fixes $k$, and its unit residue modulo three fixes $\epsilon$. Cubing is an automorphism on $\{1,-1\}$, so it remains to compute the cube map on the [principal units](../../../../../principal-unit.md).

For $t\in\mathbb Z_3$,

$$
(1+3t)^3=1+9\bigl(t+3t^2+3t^3\bigr).
$$

Thus $U_1^3\subseteq U_2:=1+9\mathbb Z_3$. Conversely, given $1+9a\in U_2$, apply [Hensel lemma](../../../../../hensel-s-lemma.md) to

$$
F(T)=T+3T^2+3T^3-a.
$$

Modulo three it is $T-a$, and $F'(T)=1+6T+9T^2$ is always a unit. The residue root $a\bmod3$ therefore lifts, giving $t$ with $(1+3t)^3=1+9a$. Hence

$$
\boxed{U_1^3=U_2.}
$$

This is the [cube map on 3-adic principal units](../../../../../cube-map-on-3-adic-principal-units.md). Introducing $T$ is essential: applying simple-root lifting directly to $X^3-u$ would fail because its derivative is divisible by three at every unit.

The map $1+3t\mapsto t\bmod3$ induces an isomorphism $U_1/U_2\cong(\mathbb Z/3\mathbb Z,+)$, since multiplication adds the first principal-unit digits modulo three. The [valuation](../../../../../valuation.md) factor contributes $\mathbb Z/3\mathbb Z$ independently, so the [cube-class group of the 3-adic numbers](../../../../../cube-class-group-of-the-3-adic-numbers.md) is

$$
\boxed{\mathbb Q_3^\times/(\mathbb Q_3^\times)^3\cong\mathbb Z/3\mathbb Z\times\mathbb Z/3\mathbb Z.}
$$

Explicit generators are the classes of $3$ and $4=1+3$. Representatives are $3^a4^b$ with $0\leq a,b<3$. The class of $3$ is detected by [valuation](../../../../../valuation.md) modulo three, and that of $4$ by its nonzero first principal-unit digit, so the two generators are independent.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 123](../../paper-123-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
