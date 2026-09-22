<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Construct an [economical two-state quantum cloner](../../../../../../economical-two-state-quantum-cloner.md) by moving both actual outputs slightly toward one another relative to the two desired copies. Set $|a\rangle=|00\rangle$ and $|b\rangle=|++\rangle$. Their overlap is $1/2$, so their sum and difference yield the [orthonormal](../../../../../../orthonormal-set.md) vectors

$$
|u\rangle=\frac{|a\rangle+|b\rangle}{\sqrt3},\qquad
|v\rangle=|a\rangle-|b\rangle.
$$

The desired outputs have the symmetric expressions

$$
|a\rangle=\cos\frac\pi6|u\rangle+\sin\frac\pi6|v\rangle,
\qquad
|b\rangle=\cos\frac\pi6|u\rangle-\sin\frac\pi6|v\rangle.
$$

Choose the actual outputs to be

$$
|c_0\rangle=\cos\frac\pi8|u\rangle+\sin\frac\pi8|v\rangle,
\qquad
|c_+\rangle=\cos\frac\pi8|u\rangle-\sin\frac\pi8|v\rangle.
$$

They are normalized and satisfy

$$
\langle c_0|c_+\rangle=\cos\frac\pi4=\frac1{\sqrt2}
=\langle00|+0\rangle.
$$

Consequently the prescription $|00\rangle\mapsto|c_0\rangle$, $|+0\rangle\mapsto|c_+\rangle$ preserves the [Gram matrix](../../../../../../gram-matrix.md) of the two inputs and defines a [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) on their span. The [unitary extension of a finite-dimensional isometry](../../../../../../unitary-extension-of-a-finite-dimensional-isometry.md) gives a [unitary operator](../../../../../../unitary-operator.md) on the same four-dimensional, two-[qubit](../../../../../../qubit.md) [Hilbert space](../../../../../../hilbert-space-split.md); no extra workspace is required.

For an explicit full-space construction, define $c=\cos(\pi/8)$, $s=\sin(\pi/8)$ and the [orthonormal basis](../../../../../../orthonormal-basis.md)

$$
|p\rangle=c|00\rangle+s|10\rangle,\qquad
|m\rangle=s|00\rangle-c|10\rangle,\qquad |01\rangle,\ |11\rangle.
$$

Choose two further [orthonormal](../../../../../../orthonormal-set.md) vectors perpendicular to $u,v$,

$$
|w\rangle=\frac{|01\rangle-|10\rangle}{\sqrt2},\qquad
|t\rangle=\frac{|01\rangle+|10\rangle-2|11\rangle}{\sqrt6}.
$$

Then

$$
U=|u\rangle\langle p|+|v\rangle\langle m|
+|w\rangle\langle01|+|t\rangle\langle11|
$$

maps one [orthonormal basis](../../../../../../orthonormal-basis.md) to another and is therefore [unitary](../../../../../../unitary-connection.md). Since $|00\rangle=c|p\rangle+s|m\rangle$ and $|+0\rangle=c|p\rangle-s|m\rangle$, it has exactly the required two outputs.

Finally,

$$
\langle a|c_0\rangle=\langle b|c_+\rangle
=\cos\frac\pi6\cos\frac\pi8+\sin\frac\pi6\sin\frac\pi8
=\cos\frac\pi{24}.
$$

Both inputs therefore have the same [global cloning fidelity](../../../../../../global-cloning-fidelity.md), and so does their average:

$$
\boxed{F_0=F_+=\overline F=\cos^2\frac\pi{24}\approx0.9829629131.}
$$

This proves the requested existence with a two-[qubit](../../../../../../qubit.md) [unitary gate](../../../../../../quantum-logic-gate.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
