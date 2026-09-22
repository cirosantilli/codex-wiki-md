<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Let $H|n\rangle=E_n|n\rangle$, with nondegenerate eigenvalues, and expand the perturbed state as $|n\rangle+\lambda|n^{(1)}\rangle+\cdots$, choosing $\langle n|n^{(1)}\rangle=0$. The first-order eigenvalue equation gives $E_n^{(1)}=V_{nn}$ and, after projection onto $m\ne n$, $\langle m|n^{(1)}\rangle=V_{mn}/(E_n-E_m)$. Projecting the second-order equation onto $n$ then gives the [second-order nondegenerate perturbation theory](../../../../../second-order-nondegenerate-perturbation-theory.md) result

$$
\boxed{E_n(\lambda)=E_n+\lambda V_{nn}+\lambda^2\sum_{m\ne n}\frac{|V_{mn}|^2}{E_n-E_m}+O(\lambda^3).}
$$

For [angular momentum](../../../../../angular-momentum.md), $j=0,1/2,1,\ldots$, $m=-j,-j+1,\ldots,j$, and $J^2|jm\rangle=j(j+1)|jm\rangle$, $J_3|jm\rangle=m|jm\rangle$ in units $\hbar=1$.

Take $H_0=-\gamma B_3J_3$ with $\gamma B_3\ne0$ and perturbation $-\gamma B_1J_1$. The diagonal matrix element of $J_1=(J_++J_-)/2$ vanishes. Only $m\pm1$ contribute at second order. Their squared matrix elements are $[j(j+1)-m(m\pm1)]/4$, and their unperturbed energy denominators are respectively $\gamma B_3$ and $-\gamma B_3$. Thus

$$
\Delta E_m^{(2)}=\frac{\gamma B_1^2}{4B_3}\{[j(j+1)-m(m+1)]-[j(j+1)-m(m-1)]\}=-\frac{\gamma mB_1^2}{2B_3}.
$$

Hence $\boxed{E_m=-\gamma B_3m-\gamma mB_1^2/(2B_3)+O(B_1^4)}$. Rotating the quantization axis to the field gives exact energies $-\gamma m_B\sqrt{B_3^2+B_1^2}$. Labeling each branch continuously from its original $m$ gives $E_m=-\gamma mB_3\sqrt{1+B_1^2/B_3^2}$, whose expansion agrees, including negative $B_3$. If $B_3=0$, the nondegenerate starting point fails and this expansion cannot be used.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
