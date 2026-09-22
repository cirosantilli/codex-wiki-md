# Economical two-state quantum cloner

↑ **Parent:** [Quantum cloning](quantum-cloning.md)

A two-[qubit](qubit.md) [unitary gate](quantum-logic-gate.md) can approximately clone the known pair $|0\rangle,|+\rangle$ with [global cloning fidelity](global-cloning-fidelity.md) $\cos^2(\pi/24)$ for each input, using no additional workspace. To construct it, put $a=|00\rangle$, $b=|++\rangle$, $u=(a+b)/\sqrt3$ and $v=a-b$. The vectors $u,v$ are [orthonormal](orthonormal-set.md), and $a,b$ have coefficients $(\cos(\pi/6),\pm\sin(\pi/6))$ in that basis. Choose output vectors with coefficients $(\cos(\pi/8),\pm\sin(\pi/8))$. Their [inner product](inner-product-split.md) is $\cos(\pi/4)=1/\sqrt2$, exactly the overlap of the inputs $|00\rangle,|+0\rangle$. Their linear matching therefore defines a [linear isometry](linear-isometry-of-hilbert-spaces.md) on the input span and extends to a two-[qubit](qubit.md) [unitary operator](unitary-operator.md) by [unitary extension of a finite-dimensional isometry](unitary-extension-of-a-finite-dimensional-isometry.md). Each output's overlap with its ideal copy is $\cos(\pi/6-\pi/8)=\cos(\pi/24)$, proving the stated [squared quantum fidelity](squared-quantum-fidelity.md).

## ↑ Ancestors (5)

1. [Quantum cloning](quantum-cloning.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information/3/d/iii/solution.md)
