# Exponent reduction for units

↑ **Parent:** [Euler's theorem](euler-s-theorem.md)

For a [unit modulo n](unit-modulo-n.md) $a$ and a [nonnegative integer](natural-number.md) $k$, [division with remainder](euclidean-division.md) writes $k=q\varphi(n)+r$ with $0\leq r<\varphi(n)$. [Euler's theorem](euler-s-theorem.md) then gives

$$
a^k=(a^{\varphi(n)})^q a^r\equiv a^r\pmod n.
$$

This replaces a potentially enormous [exponent](exponent.md) by a small [remainder](remainder.md). The [exponent](exponent.md) itself is reduced modulo [Euler's totient function](euler-totient-function.md), while the powers are reduced modulo $n$: these are different [integer moduli](modulus-in-modular-arithmetic.md).

For a worked modulo-fifteen calculation, seven is [coprime](coprime-integers.md) to fifteen and $\varphi(15)=8$. Therefore

$$
2029=253\cdot8+5,\qquad 7^{2029}\equiv7^5\pmod{15}.
$$

Use [exponentiation by squaring](exponentiation-by-squaring.md) on the remaining [exponent](exponent.md) $5=(101)_2$, reducing after each [multiplication](multiplication.md):

$$
7^2\equiv49\equiv4,\qquad
7^4\equiv4^2\equiv1,\qquad
7^5\equiv1\cdot7\equiv7\pmod{15}.
$$

Thus **$7^{2029}\bmod15=7$**. [Modular exponentiation](modular-exponentiation.md) supplies the computation; [Euler's theorem](euler-s-theorem.md) supplies the optional shortening of its [exponent](exponent.md). [Exponentiation by squaring](exponentiation-by-squaring.md) also works for [nonunit](nonunit.md) bases, without using this shortening.

The guaranteed [exponent](exponent.md) $\varphi(n)$ is a common return [exponent](exponent.md) and an upper bound on the shortest period; it need not be that period. The [multiplicative order](multiplicative-order.md) $d=\operatorname{ord}_n(a)$ is the least positive return [exponent](exponent.md) for the chosen [unit](unit-in-a-ring.md). The [Carmichael function](carmichael-function.md) $\lambda(n)$ is the least positive return [exponent](exponent.md) that works for every [unit](unit-in-a-ring.md). Their precise relation is

$$
\operatorname{ord}_n(a)\mid\lambda(n)\mid\varphi(n).
$$

Either smaller return [exponent](exponent.md) can replace $\varphi(n)$ in [exponent reduction for units](exponent-reduction-for-units.md). Modulo fifteen, $\operatorname{ord}_{15}(7)=\lambda(15)=4<8=\varphi(15)$, so $2029=507\cdot4+1$ gives $7^{2029}\equiv7$ immediately. For base four the [multiplicative order](multiplicative-order.md) is only two, smaller even than $\lambda(15)$. A return at [exponent](exponent.md) eight alone does not prove that the [multiplicative order](multiplicative-order.md) is eight.[pp. 1–3, Definition 1.3, the warning on p. 2, Theorem 2.1, Corollary 2.2 and Theorem 2.4](orders-of-units-in-modular-arithmetic-by-keith-conrad.md)

<a id="image-actual-power-periods-carmichael-function-exponents-and-euler-return-exponents"></a>
![](euler-unit-powers-and-exponent-periods.png)

**[Figure 39](#image-actual-power-periods-carmichael-function-exponents-and-euler-return-exponents). Actual power periods, Carmichael function exponents and Euler return exponents**. Each row lists powers from exponent zero through eight. Highlighted first returns identify [multiplicative orders](multiplicative-order.md); the accompanying labels distinguish a chosen base's shortest period, the common exponent for all [units](unit-in-a-ring.md), and [Euler's totient function](euler-totient-function.md). Powers of the [nonunit](nonunit.md) three modulo fifteen repeat after an initial term but never return to one at a positive exponent. The final calculation compares reduction of $2029$ modulo eight and modulo four.

If the reduced [exponent](exponent.md) is zero, the rule gives $a^k\equiv a^0=1$, and still requires a [unit](unit-in-a-ring.md). Applying it to the [nonunit](nonunit.md) three would falsely predict $3^8\equiv3^0=1\pmod{15}$; the actual residue is six. For negative [exponents](exponent.md), first interpret the power using a [modular multiplicative inverse](modular-multiplicative-inverse.md), as in [modular exponentiation](modular-exponentiation.md).

## ↑ Ancestors (5)

1. [Euler's theorem](euler-s-theorem.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Euler's theorem](euler-s-theorem.md)
- [Exponent reduction for units](exponent-reduction-for-units.md)
