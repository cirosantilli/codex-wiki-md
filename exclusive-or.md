# Exclusive or

↑ **Parent:** [Boolean operation](boolean-operation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exclusive_or)

[Exclusive or](exclusive-or.md) returns one exactly when its two input [bits](bit.md) differ. Its [truth table](truth-table.md) gives $0\oplus0=0$, $0\oplus1=1$, $1\oplus0=1$, and $1\oplus1=0$. The identities

$$
P\oplus Q=(P\vee Q)\wedge\neg(P\wedge Q)
=(P\wedge\neg Q)\vee(\neg P\wedge Q)
$$

express [exclusive or](exclusive-or.md) using [logical conjunction](logical-conjunction.md), [logical disjunction](logical-disjunction.md), and [logical negation](negation.md). The first expression accepts at least one input and then excludes both; the second explicitly lists the two accepted input pairs.

For numerical [bits](bit.md), [exclusive or](exclusive-or.md) is [addition](addition.md) in [modular arithmetic](modular-arithmetic-split.md) modulo two:

$$
x\oplus y=(x+y)\bmod2.
$$

The [binary operation](binary-operation.md) is [commutative](commutativity.md) and [associative](associative-property.md), because [addition](addition.md) modulo two has those properties. It satisfies $x\oplus0=x$, $x\oplus1=\neg x$, and $x\oplus x=0$. These identities explain why a [bit](bit.md) can be toggled and restored with the same operation.

On [binary strings](binary-string.md) of equal length, bitwise [exclusive or](exclusive-or.md) applies the one-[bit](bit.md) rule separately at each position. For example,

$$
1010\oplus0110=1100,\qquad1100\oplus0110=1010.
$$

A [bit mask](bit-mask.md) of $0110$ toggles exactly the middle two [bits](bit.md). Applying the mask twice restores the original [binary string](binary-string.md): each selected [bit](bit.md) changes twice, and each unselected [bit](bit.md) stays fixed. This positional operation is distinct from taking the [exclusive or](exclusive-or.md) of the overall [truth values](truth-value.md) of two [integers](integer-split.md).

**Table of contents**

- [Exclusive or toggles and parity](exclusive-or-toggles-and-parity.md)

## ↑ Ancestors (4)

1. [Boolean operation](boolean-operation.md)
2. [Theoretical computer science](theoretical-computer-science-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (65)

- [Algebraic normal form](algebraic-normal-form.md)
- [Binary rate-distortion function](binary-rate-distortion-function.md)
- [Binary symmetric channel](binary-symmetric-channel.md)
- [Boolean operation](boolean-operation.md)
- [Boolean operations on events](boolean-operations-on-events.md)
- [Carryless multiplication](carryless-multiplication.md)
- [Chain rule for mutual information](chain-rule-for-mutual-information.md)
- [CHSH game](chsh-game.md)
- [Classical query complexity of linear Boolean function identification](classical-query-complexity-of-linear-boolean-function-identification.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Conditioning can destroy independence](conditioning-can-destroy-independence.md)
- [Correlated binary variables](correlated-binary-variables.md)
- [Data processing inequality](data-processing-inequality.md)
- [Exclusive or](exclusive-or.md)
- [Exclusive-or natural deduction rules](exclusive-or-natural-deduction-rules.md)
- [Exclusive or toggles and parity](exclusive-or-toggles-and-parity.md)
- [Function oracle](function-oracle.md)
- [GHZ game](ghz-game.md)
- [Grundy number](grundy-number.md)
- [Half adder](half-adder.md)
- [Innovations in a binary Markov source](innovations-in-a-binary-markov-source.md)
- [Linear Boolean function](linear-boolean-function.md)
- [Mutual information](mutual-information.md)
- [Nim](nim.md)
- [Nim-sum](nim-sum.md)
- [NOR gate](nor-gate.md)
- [Pairwise independence does not imply joint independence](pairwise-independence-does-not-imply-joint-independence.md)
- [Pairwise independent events](pairwise-independent-events.md)
- [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)
- [Parity lower bound for Boolean queries](parity-lower-bound-for-boolean-queries.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-networks/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-networks/1/g/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-security/3/b/ii/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/2/c/solution.md)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2015/1/b/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8/8/1/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/5/1/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/1/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2019/5/b/ii/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2019/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/4/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/4/b/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/6/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/digital-systems-linear-algebra-introduction-to-formal-proof/7/d/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/3/b/solution.md)
- [Phase oracle](phase-oracle.md)
- [Quantum collision finding](quantum-collision-finding.md)
- [Quantum oracle](quantum-oracle.md)
- [Rule 90](rule-90.md)
- [Separated Boolean decomposition](separated-boolean-decomposition.md)
- [Sprague-Grundy theorem](sprague-grundy-theorem.md)
- [Three-bit majority decision tree](three-bit-majority-decision-tree.md)
- [XOR separation by a product feature](xor-separation-by-a-product-feature.md)
