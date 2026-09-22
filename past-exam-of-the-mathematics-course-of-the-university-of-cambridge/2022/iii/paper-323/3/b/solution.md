<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Data processing states $D(\Phi(\rho)\|\Phi(\sigma))\leq D(\rho\|\sigma)$ for every quantum channel $\Phi$. Joint convexity states

$$
D\left(\sum_ip_i\rho_i\middle\|\sum_ip_i\sigma_i\right)
\leq\sum_ip_iD(\rho_i\|\sigma_i).
$$

Strong subadditivity states $S(ABC)+S(B)\leq S(AB)+S(BC)$.

For strong subadditivity, apply data processing under $\operatorname{Tr}_C$ to $\rho_{ABC}$ and $I_A/d_A\otimes\rho_{BC}$. Expanding both relative entropies cancels $\log d_A$ and gives precisely the stated inequality. For joint convexity, use flagged states $\widehat\rho=\sum_ip_i|i\rangle\langle i|\otimes\rho_i$ and $\widehat\sigma=\sum_ip_i|i\rangle\langle i|\otimes\sigma_i$. Part a gives $D(\widehat\rho\|\widehat\sigma)=\sum_ip_iD(\rho_i\|\sigma_i)$; discarding the flag and applying data processing gives [joint convexity of quantum relative entropy](../../../../../../joint-convexity-of-quantum-relative-entropy.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
