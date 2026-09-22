# Exclusive or toggles and parity

↑ **Parent:** [Exclusive or](exclusive-or.md)

For [bits](bit.md) $x_1,\ldots,x_n$, repeated [exclusive or](exclusive-or.md) computes the [parity](parity.md) of the number of ones:

$$
x_1\oplus\cdots\oplus x_n=\left(\sum_{i=1}^n x_i\right)\bmod2.
$$

An [induction](mathematical-induction.md) proves this: the first [bit](bit.md) gives its own [parity](parity.md), and appending a zero preserves it while appending a one changes it. The [binary string](binary-string.md) $10110$ has three ones, so its [parity bit](parity-bit.md) is one. Append that [parity bit](parity-bit.md) to obtain $101101$, whose six [bits](bit.md) have even [parity](parity.md). Flipping the second [bit](bit.md) produces $111101$ and changes the combined [exclusive or](exclusive-or.md) to one, detecting an error. Flipping the third [bit](bit.md) as well produces $110101$, with four ones and combined [exclusive or](exclusive-or.md) zero: an even number of flips can escape this check.

For three inputs, repeated [exclusive or](exclusive-or.md) means an odd number of true inputs, rather than exactly one: $1\oplus1\oplus1=1$. The “exactly one” description applies to the two-input [exclusive or](exclusive-or.md). This distinction matters when translating a requirement that exactly one option be selected into a program condition.

## ↑ Ancestors (5)

1. [Exclusive or](exclusive-or.md)
2. [Boolean operation](boolean-operation.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
