# One-qubit reduction of Dicke-state superpositions

↑ **Parent:** [Dicke state](dicke-state.md)

For $|\Omega\rangle=\alpha|D_m^n\rangle+\beta|D_{m+1}^n\rangle$, $|\alpha|^2+|\beta|^2=1$ and $0\leq m<n$, the [reduced density matrix](reduced-density-matrix.md) of any one qubit is

$$
\rho=\frac1n\begin{pmatrix}(n-m)|\alpha|^2+(n-m-1)|\beta|^2&\sqrt{(n-m)(m+1)}\,\alpha\beta^*\\\sqrt{(n-m)(m+1)}\,\alpha^*\beta&m|\alpha|^2+(m+1)|\beta|^2\end{pmatrix}.
$$

Use the [Dicke state](dicke-state.md) recursion. The rest-of-system vectors of different [Hamming weights](hamming-weight.md) are orthogonal. For the diagonal terms this leaves the probabilities of the distinguished bit being zero and one. In the cross term, only the rest vector $|D_m^{n-1}\rangle$ occurs in both states, with coefficients $\sqrt{(n-m)/n}$ multiplying $|0\rangle$ and $\sqrt{(m+1)/n}$ multiplying $|1\rangle$. Thus $\operatorname{Tr}_{\mathrm{rest}}(|D_m^n\rangle\langle D_{m+1}^n|)=\sqrt{(n-m)(m+1)}|0\rangle\langle1|/n$, proving the matrix. A single [Dicke state](dicke-state.md) alone gives the diagonal matrix $\operatorname{diag}((n-m)/n,m/n)$.

## ↑ Ancestors (7)

1. [Dicke state](dicke-state.md)
2. [Quantum state](quantum-state.md)
3. [Quantum system](quantum-system.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Dicke-resource telecloning](dicke-resource-telecloning.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/1/c/solution.md)
