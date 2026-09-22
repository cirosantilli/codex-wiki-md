# Coherent-state photon statistics

↑ **Parent:** [Photon statistics](photon-statistics.md)

For a [coherent state](coherent-state.md), write $a|\alpha\rangle=\alpha|\alpha\rangle$ and $|\alpha\rangle=\sum_n c_n|n\rangle$ in [number states](number-state.md). The [annihilation operator](annihilation-operator.md) gives $c_{n+1}\sqrt{n+1}=\alpha c_n$, so $c_n=c_0\alpha^n/\sqrt{n!}$. Normalization yields $|c_0|^2=e^{-|\alpha|^2}$. Thus [photon statistics](photon-statistics.md) follows a [Poisson distribution](poisson-distribution.md) with $\mu=|\alpha|^2$, and the [normal ordering](normal-ordering.md) of every moment gives $\langle(a^\dagger)^ka^k\rangle=\mu^k$. This factorization is the defining virtue of [coherent states](coherent-state.md) for optical calculations.[1963, §III, equations (3.1)–(3.7): coherent-state expansion; Universidade Estadual de Campinas mirror](coherent-and-incoherent-states-of-the-radiation-field-by-roy-jay-glauber.md)

As an original comparison, choose $\mu=2$. Then $p_0=e^{-2}$, $p_1=p_2=2e^{-2}$, $\operatorname{Var}N=2$, and $\langle N(N-1)\rangle=4$. A two-[photon](photon.md) [Fock state](fock-state.md) also has mean two but has $\operatorname{Var}N=0$ and pair moment two. Consequently

$$
g^{(2)}_{\rm coherent}(0)=1,\qquad
g^{(2)}_{|n\rangle}(0)=1-\frac1n\quad(n\geq1).
$$

In particular, $|1\rangle$ cannot supply a pair. Nevertheless, [photon statistics](photon-statistics.md) alone does not determine a [quantum state](quantum-state.md): averaging $|\alpha\rangle\langle\alpha|$ over a uniform [quantum phase](quantum-phase.md) removes its off-diagonal entries while retaining exactly the same $p_n$ and these equal-time moments.

## ↑ Ancestors (6)

1. [Photon statistics](photon-statistics.md)
2. [Quantum optics](quantum-optics-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
