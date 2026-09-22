# Heisenberg exchange echo

↑ **Parent:** [Quantum control](quantum-control.md)

For $H=J(XX+YY+ZZ)/2$, $U=e^{-itH}$, and an individually applied [Pauli Z gate](pauli-z-gate.md) $P=Z\otimes I$, conjugation gives $PHP=J(-XX-YY+ZZ)/2$. The paired [Pauli operators](pauli-operator.md) $XX,YY,ZZ$ commute with one another, so

$$
PUPU=e^{-itPHP}e^{-itH}=e^{-iJtZZ}.
$$

Two equal free-evolution intervals, each of duration $t$, therefore cancel exchange while retaining the [Ising coupling](ising-coupling-of-two-qubits.md). This [spin echo](spin-echo.md) is exact for instantaneous ideal gates; a finite pulse requires accounting for the interaction during the pulse. A simultaneous [Pauli Z gate](pauli-z-gate.md) on each spin commutes with $H$ and cannot perform the same cancellation. The physical availability of the individual gate is a separate [quantum control](quantum-control.md) requirement.

## ↑ Ancestors (5)

1. [Quantum control](quantum-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2008/6/2/solution.md)
