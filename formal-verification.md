# Formal verification

↑ **Parent:** [Algorithm correctness](algorithm-correctness.md)

Establishing specified properties of a system using [formal proofs](formal-proof.md) about a precise model. [Formal verification](formal-verification.md) connects an implementation to a [formal specification](formal-specification.md); correctness of the model and its assumptions still matters when applying the result to a physical system.

For a small example, the [summation loop verification](summation-loop-verification.md) below starts with executable steps and asks two separate questions: does any returned value satisfy the [postcondition](postcondition.md), and does execution reach that return? A [loop invariant](loop-invariant.md) answers the first; a [loop variant](loop-variant.md) answers the second. This turns an unbounded family of permitted [inputs](input-computer-science.md) into a few reusable proof obligations.

The model must specify [programming language semantics](programming-language-semantics.md), including the meaning of [variable assignments](variable-assignment.md), comparisons and [integer arithmetic](integer-arithmetic.md). A proof about exact mathematical [integers](integer-split.md) need not describe a machine that wraps on [integer overflow](integer-overflow.md). Similarly, a correct [formal proof](formal-proof.md) of a weak or mistaken [formal specification](formal-specification.md) does not establish the intended behavior. Choosing the right [formal specification](formal-specification.md) and relating the model to the implemented system remain substantive tasks.

[Software testing](software-testing.md) examines chosen executions and can expose a [counterexample](counterexample.md). A [formal proof](formal-proof.md) instead justifies a statement throughout its stated model; it does not require executing every permitted [input](input-computer-science.md). This makes [formal verification](formal-verification.md) valuable when rare boundary cases matter, while [software testing](software-testing.md) can still reveal an incorrect model or misunderstood requirement.

In 1969, [Tony Hoare](tony-hoare.md) presented rules for [variable assignment](variable-assignment.md), composition and iteration in a small [programming language](programming-language-split.md). His paper explicitly says those rules do not prove successful termination, and discusses the dependence of arithmetic reasoning on the chosen overflow behavior. These reservations already make the model's scope part of the argument.[Hoare, An Axiomatic Basis for Computer Programming, §2 Computer Arithmetic, pp. 576–577; §§3.1–3.4, pp. 577–578; §4 General Reservations, pp. 578–579](an-axiomatic-basis-for-computer-programming-by-tony-hoare.md)

**Table of contents**

- [Summation loop verification](summation-loop-verification.md)
- [Formal specification](formal-specification.md)
  - [Precondition](precondition.md)
  - [Postcondition](postcondition.md)
- [Binary correctness](binary-correctness.md)

## ↑ Ancestors (4)

1. [Algorithm correctness](algorithm-correctness.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Binary correctness](binary-correctness.md)
- [Formal verification](formal-verification.md)
- [seL4 verification scope](sel4-verification-scope.md)
