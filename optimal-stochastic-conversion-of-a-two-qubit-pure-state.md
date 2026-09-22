# Optimal stochastic conversion of a two-qubit pure state

↑ **Parent:** [Local operations and classical communication](local-operations-and-classical-communication.md)

Write a source and target in [Schmidt decomposition](schmidt-decomposition.md) with squared coefficients $(1-s,s)$ and $(1-t,t)$, where $0<s,t\leq1/2$. If $s\geq t$, [Nielsen's pure-state conversion theorem](nielsen-s-pure-state-conversion-theorem.md) allows deterministic conversion. If $s<t$, the [Schmidt-tail entanglement monotone](schmidt-tail-entanglement-monotone.md) gives $p\leq s/t$. Alice attains this bound with a local two-outcome [measurement in quantum mechanics](quantum-measurement-split.md) whose success [Kraus operator](kraus-operator.md) is $K_s=\operatorname{diag}(\sqrt{s(1-t)/(t(1-s))},1)$ and whose failure operator is $K_f=\operatorname{diag}(\sqrt{1-s(1-t)/(t(1-s))},0)$. They obey $K_s^\dagger K_s+K_f^\dagger K_f=I$. The successful unnormalized state is $\sqrt{s/t}$ times the target, and failure leaves a [product state](product-state.md). A classical message tells Bob which branch occurred. Known local changes of Schmidt bases allow the same protocol for arbitrary two-qubit pure states with these coefficients.

## ↑ Ancestors (6)

1. [Local operations and classical communication](local-operations-and-classical-communication.md)
2. [Bell state](bell-state-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Collective advantage over independent two-qubit filtering](collective-advantage-over-independent-two-qubit-filtering.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/c/solution.md)
