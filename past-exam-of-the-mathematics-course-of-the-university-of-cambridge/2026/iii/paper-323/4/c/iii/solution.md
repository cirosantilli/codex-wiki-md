<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $q=(1+\varepsilon)^{-1}$, so $1-q=\varepsilon/(1+\varepsilon)$ and $\omega=q\rho+(1-q)\Delta'$. For every state $\xi_B$, the [entropy bound for a binary mixture](../../../../../../../entropy-bound-for-a-binary-mixture.md) gives

$$
\begin{aligned}
D(\omega_{AB}\|I_A\otimes\xi_B)
&=-S(\omega_{AB})-\operatorname{Tr}(\omega_B\log\xi_B)\\
&\geq qD(\rho_{AB}\|I_A\otimes\xi_B)
 +(1-q)D(\Delta'_{AB}\|I_A\otimes\xi_B)-H(q).
\end{aligned}
$$

Taking the minimum over $\xi_B$ and using the [variational characterization of quantum conditional entropy](../../../../../../../variational-characterization-of-quantum-conditional-entropy.md) on each term gives

$$
-H(A|B)_\omega
\geq-qH(A|B)_\rho-(1-q)H(A|B)_{\Delta'}-H(q).
$$

Since [binary entropy](../../../../../../../binary-entropy.md) satisfies $H(q)=H(1-q)$, this is

$$
\boxed{H(A|B)_\omega\leq
\frac{H(A|B)_\rho+\varepsilon H(A|B)_{\Delta'}}{1+\varepsilon}
+H\!\left(\frac{\varepsilon}{1+\varepsilon}\right)}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
