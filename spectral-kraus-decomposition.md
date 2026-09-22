# Spectral Kraus decomposition

↑ **Parent:** [Choi matrix](choi-matrix.md)

Use the unnormalized [Choi matrix](choi-matrix.md) $J(\Phi)=(\Phi\otimes\mathrm{id})(|\widetilde\Psi\rangle\langle\widetilde\Psi|)$, which has trace $d$ for a channel. A positive such matrix has a spectral decomposition with vectors $v_k=\sqrt{\lambda_k}u_k$. In paired bases define the [Kraus operator](kraus-operator.md) $A_k$ by $(A_k)_{ij}=(v_k)_{ij}$, so $v_k=(A_k\otimes I)\sum_j|j\rangle|j\rangle$. Partial contraction with a [conjugate index vector](conjugate-index-vector.md) gives $A_k|\phi\rangle$, hence $\Phi(|\phi\rangle\langle\phi|)=\sum_kA_k|\phi\rangle\langle\phi|A_k^\dagger$. Rank-one projectors span the operator space, proving the [Kraus representation](kraus-representation.md) on all inputs. Trace preservation is equivalent to $\sum_kA_k^\dagger A_k=I$. This construction needs at most $\operatorname{rank}J$ nonzero Kraus operators.

## ↑ Ancestors (8)

1. [Choi matrix](choi-matrix.md)
2. [Completely positive map](completely-positive-map.md)
3. [Positive linear map](positive-linear-map.md)
4. [Quantum information theory](quantum-information-theory-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34/4/d/solution.md)
