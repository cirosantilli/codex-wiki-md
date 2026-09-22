# Finite-state machine

↑ **Parent:** [Formal language theory](formal-language-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite-state_machine)

A [finite-state machine](finite-state-machine.md) processes inputs using a [finite set](finite-set.md) of [automaton states](automaton-state.md) and input-dependent [automaton transitions](automaton-transition.md). An [automaton state](automaton-state.md) records everything the machine remembers; an [automaton transition](automaton-transition.md) says how that memory changes on the next symbol. A [finite-state machine](finite-state-machine.md) may also emit outputs. Here the emphasis is on recognizing a [formal language](formal-language.md): start in a designated [automaton state](automaton-state.md), read a [word](string.md) from an [alphabet](alphabet.md), and accept exactly when the final [automaton state](automaton-state.md) is designated accepting.

Finite memory does not impose a maximum input length. A [finite-state machine](finite-state-machine.md) can read arbitrarily long [words](string.md), revisiting its [automaton states](automaton-state.md) indefinitely. The restriction is that the part already read must be compressed into one of finitely many summaries. For [divisibility](divisibility.md) by three, a [word](string.md) of [binary digits](binary-digit.md) can describe an enormous [integer](integer.md), yet its [congruence class](congruence-class.md) modulo three is all that the machine needs to retain. Two already-read [words](string.md) giving the same [automaton state](automaton-state.md) behave identically under every subsequent continuation in a [DFA](deterministic-finite-automaton.md).

This makes [finite-state machines](finite-state-machine.md) useful whenever past details can be forgotten safely: checking whether a sequence of commands follows an allowed order, or recognizing a pattern with a [regular expression](regular-expression.md). The beautiful design question is which distinctions about the past matter to the future. [DFA minimization](dfa-minimization.md) makes that question precise by merging [indistinguishable states of a deterministic finite automaton](indistinguishable-states-of-a-deterministic-finite-automaton.md). Both [DFAs](deterministic-finite-automaton.md) and [NFAs](nondeterministic-finite-automaton.md) recognize exactly the [regular languages](regular-language.md).

**Table of contents**

- [Automaton state](automaton-state.md)
- [Automaton transition](automaton-transition.md)
- [Dead state of a finite automaton](dead-state-of-a-finite-automaton.md)
- [Generalized finite automaton](generalized-finite-automaton.md)
  - [State elimination for finite automata](state-elimination-for-finite-automata.md)
    - [Finite-state path expression](finite-state-path-expression.md)
- [Deterministic finite automaton](deterministic-finite-automaton.md)
  - [Extended transition function of a deterministic finite automaton](extended-transition-function-of-a-deterministic-finite-automaton.md)
  - [Accessible state of a deterministic finite automaton](accessible-state-of-a-deterministic-finite-automaton.md)
  - [Indistinguishable states of a deterministic finite automaton](indistinguishable-states-of-a-deterministic-finite-automaton.md)
    - [Quotient deterministic finite automaton by indistinguishable states](quotient-deterministic-finite-automaton-by-indistinguishable-states.md)
  - [Irreducible deterministic finite automaton](irreducible-deterministic-finite-automaton.md)
  - [Parity-counting deterministic finite automaton](parity-counting-deterministic-finite-automaton.md)
  - [Bounded-run deterministic finite automaton](bounded-run-deterministic-finite-automaton.md)
  - [DFA minimization](dfa-minimization.md)
    - [Minimal deterministic finite automaton](minimal-deterministic-finite-automaton.md)
      - [Canonical residual automaton](canonical-residual-automaton.md)
      - [Cycle state in a minimal deterministic finite automaton for a finite language](cycle-state-in-a-minimal-deterministic-finite-automaton-for-a-finite-language.md)
      - [Binary divisibility automaton](binary-divisibility-automaton.md)
      - [Accessible unary deterministic finite automaton](accessible-unary-deterministic-finite-automaton.md)
- [Nondeterministic finite automaton](nondeterministic-finite-automaton.md)
  - [Epsilon-NFA](epsilon-nfa.md)
    - [Epsilon closure](epsilon-closure.md)
    - [Subset construction with epsilon transitions](subset-construction-with-epsilon-transitions.md)
  - [Extended transition of a nondeterministic finite automaton](extended-transition-of-a-nondeterministic-finite-automaton.md)
    - [Witnessing sequence for a nondeterministic automaton](witnessing-sequence-for-a-nondeterministic-automaton.md)
  - [Powerset construction](powerset-construction.md)
  - [Brzozowski automaton](brzozowski-automaton.md)
    - [Irreducibility of the accessible subset automaton](irreducibility-of-the-accessible-subset-automaton.md)

## ↑ Ancestors (5)

1. [Formal language theory](formal-language-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Automaton state](automaton-state.md)
- [Buffer cache state model](buffer-cache-state-model.md)
- [Finite-state machine](finite-state-machine.md)
- [Nondeterministic finite automaton](nondeterministic-finite-automaton.md)
