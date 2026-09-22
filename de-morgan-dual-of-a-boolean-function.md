# De Morgan dual of a Boolean function

↑ **Parent:** [De Morgan's laws](de-morgan-s-laws.md)

For a [Boolean function](boolean-function.md) $f$ of $n$ input [bits](bit.md), define its [De Morgan dual](de-morgan-dual-of-a-boolean-function.md) by complementing every input, applying $f$, and complementing the output:

$$
f^*(x_1,\ldots,x_n)=1-f(1-x_1,\ldots,1-x_n).
$$

[De Morgan's laws](de-morgan-s-laws.md) say that the [De Morgan dual](de-morgan-dual-of-a-boolean-function.md) of [logical conjunction](logical-conjunction.md) is [logical disjunction](logical-disjunction.md), and conversely. The constant zero [Boolean function](boolean-function.md) becomes constant one. This is different from merely negating the output: for AND, output [logical negation](negation.md) gives one at $(0,0)$, whereas the [De Morgan dual](de-morgan-dual-of-a-boolean-function.md) gives zero there.

Taking the [De Morgan dual](de-morgan-dual-of-a-boolean-function.md) twice restores the original [Boolean function](boolean-function.md):

$$
(f^*)^*(x)=1-\bigl(1-f(x)\bigr)=f(x).
$$

Here each input is complemented twice as well. For a [Boolean formula](boolean-formula.md) built from AND, OR, NOT and constants, its [De Morgan dual](de-morgan-dual-of-a-boolean-function.md) can therefore be obtained by exchanging AND with OR and zero with one throughout, leaving input names and NOT in place. A structural [induction](mathematical-induction.md) proves the rule: it holds for an input and each constant, [De Morgan's laws](de-morgan-s-laws.md) handle the two binary [logical connectives](logical-connective.md), and double [logical negation](negation.md) handles NOT. This symmetry lets one translate a complex test systematically instead of guessing where its failures occur.

## ↑ Ancestors (5)

1. [De Morgan's laws](de-morgan-s-laws.md)
2. [Boolean operation](boolean-operation.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
