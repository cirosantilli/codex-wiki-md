# Hadamard transform

↑ **Parent:** [Quantum theory](quantum-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hadamard_transform)

The normalized [Hadamard transform](hadamard-transform.md) maps a [vector](vector.md) indexed by [binary strings](binary-string.md) through entries $2^{-n/2}(-1)^{x\cdot y}$, where the [dot product](dot-product.md) is evaluated modulo two. It is its own inverse and an [orthogonal transformation](orthogonal-transformation.md), hence also a [unitary operator](unitary-operator.md) on complex input vectors. The [Hadamard gate](hadamard-gate.md) is the $n=1$ quantum case, and the [Hadamard basis](hadamard-basis.md) is the image of the [computational basis](computational-basis.md). The [Walsh-Hadamard transform](walsh-hadamard-transform.md) gives the same [tensor product](tensor-product.md) construction.

For two [qubits](qubit.md), applying one [Hadamard gate](hadamard-gate.md) to each prepares the [uniform quantum superposition](uniform-quantum-superposition.md)

$$
H^{\otimes2}|00\rangle=\tfrac12(|00\rangle+|01\rangle+|10\rangle+|11\rangle).
$$

Each [probability amplitude](probability-amplitude.md) is $1/2$, so each [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) outcome has [probability](probability.md) $1/4$. Applying the [Hadamard transform](hadamard-transform.md) again reconstructs $|00\rangle$: signed contributions cancel at the other three outputs. Its usefulness lies in combining simple local [quantum gates](quantum-logic-gate.md) into an operation on exponentially many amplitudes. Extracting useful information still requires an appropriate subsequent transformation and measurement.

**Table of contents**

- [Fast Hadamard transform](fast-hadamard-transform.md)
- [Hadamard gate](hadamard-gate.md)
  - [Hadamard-phase-Hadamard qubit rotation](hadamard-phase-hadamard-qubit-rotation.md)
  - [Photon-number reference for a Hadamard gate](photon-number-reference-for-a-hadamard-gate.md)
  - [Uniform quantum superposition](uniform-quantum-superposition.md)
- [Walsh-Hadamard transform](walsh-hadamard-transform.md)
- [Hadamard basis](hadamard-basis.md)

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Amplitude amplification](amplitude-amplification.md)
- [Fourier-Walsh transform](fourier-walsh-transform.md)
- [Hadamard transform](hadamard-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/c/solution.md)
- [Walsh-Hadamard transform](walsh-hadamard-transform.md)
- [XOR convolution](xor-convolution.md)
