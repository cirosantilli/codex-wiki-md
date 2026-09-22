# Finite oscillator commutator boundary defect

↑ **Parent:** [Matrix mechanics](matrix-mechanics.md)

Retain the first $N\ge2$ [number states](number-state.md) of a [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md). Let $\Pi_N$ be the [orthogonal projection](orthogonal-projection.md) onto their span and compress $X_N=\Pi_NX\Pi_N$, $P_N=\Pi_NP\Pi_N$, restricted to this span. The compressed [annihilation operator](annihilation-operator.md) $a_N$ satisfies

$$
a_N|n\rangle=\sqrt n|n-1\rangle,\qquad a_N^\dagger|N-1\rangle=0,\qquad [a_N,a_N^\dagger]=I_N-N|N-1\rangle\langle N-1|.
$$

For $n<N-1$, the two products give $n+1$ and $n$; on the top state they give $0$ and $N-1$. Thus, with $\ell=\sqrt{\hbar/(m\omega)}$,

$$
X_N=\frac{\ell}{\sqrt2}(a_N+a_N^\dagger),\qquad P_N=\frac{i\hbar}{\sqrt2\ell}(a_N^\dagger-a_N),\qquad [X_N,P_N]=i\hbar(I_N-N|N-1\rangle\langle N-1|).
$$

On every [quantum superposition](quantum-superposition.md) of $|0\rangle,\ldots,|N-2\rangle$, this [commutator](commutator.md) acts exactly as $i\hbar I_N$. For a normalized retained state with coefficients $c_n$,

$$
\frac{\langle[X_N,P_N]\rangle}{i\hbar}=1-N|c_{N-1}|^2.
$$

Small probability at the cutoff must therefore be judged relative to $1/N$ for this expectation. For $N=8$, the diagonal of $[X_N,P_N]/(i\hbar)$ is $(1,1,1,1,1,1,1,-7)$, with zero [trace](matrix-trace.md).

<a id="image-compressed-quantum-harmonic-oscillator-matrices-and-their-exact-commutator-boundary-defect"></a>
![](oscillator-matrix-commutator-cutoff.png)

**[Figure 2](#image-compressed-quantum-harmonic-oscillator-matrices-and-their-exact-commutator-boundary-defect). Compressed quantum harmonic oscillator matrices and their exact commutator boundary defect**. Original calculation with eight retained [number states](number-state.md). Seven diagonal entries reproduce the [canonical commutation relation](canonical-commutation-relation.md); the last compensates their [trace](matrix-trace.md). The missing raising path through $|8\rangle$ creates the defect.

This is unavoidable for finite [matrices](matrix.md): [trace of a matrix commutator](trace-of-a-matrix-commutator.md) gives $\operatorname{tr}(XP-PX)=0$, whereas $\operatorname{tr}(i\hbar I_N)=i\hbar N\ne0$. Compression does not preserve products: $\Pi_NXP\Pi_N$ can use intermediate states outside the retained span, while $X_NP_N$ cannot. Accordingly, compressing the full oscillator [Hamiltonian operator](hamiltonian-quantum-mechanics.md) gives $\Pi_NH\Pi_N=\hbar\omega(a_N^\dagger a_N+I_N/2)$, but building it from the compressed squares gives

$$
\frac{P_N^2}{2m}+\frac{m\omega^2X_N^2}{2}=\Pi_NH\Pi_N-\frac{N\hbar\omega}{2}|N-1\rangle\langle N-1|.
$$

The two prescriptions agree on lower [number states](number-state.md) and disagree at the boundary. In the infinite oscillator, the [canonical commutation relation](canonical-commutation-relation.md) holds on the common invariant [dense subspace](dense-subspace.md) of finite [number state](number-state.md) combinations. Its unbounded [position](position.md) and [momentum operators](momentum-operator.md) do not admit the finite [trace](matrix-trace.md) argument; writing the formal identity does not assert that both products act on every vector of the [Hilbert space](hilbert-space-split.md).

## ↑ Ancestors (6)

1. [Matrix mechanics](matrix-mechanics.md)
2. [Operator formalism](operator-formalism.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Matrix mechanics](matrix-mechanics.md)
