<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an ensemble $\mathcal E=\{p_i,\rho_i\}$, write its channel-output [Holevo quantity](../../../../../../holevo-quantity.md) as

$$
\chi(\Phi,\mathcal E)=S\!\left(\sum_i p_i\Phi(\rho_i)\right)-\sum_i p_iS(\Phi(\rho_i)),
\qquad
\chi^*(\Phi)=\sup_{\mathcal E}\chi(\Phi,\mathcal E).
$$

Take ensembles $\mathcal E_1=\{p_i,\rho_i\}$ and $\mathcal E_2=\{q_j,\sigma_j\}$ independently, giving the product ensemble $\{p_iq_j,\rho_i\otimes\sigma_j\}$. Its average output factors:

$$
\sum_{i,j}p_iq_j\,\Phi_1(\rho_i)\otimes\Phi_2(\sigma_j)
=\left(\sum_i p_i\Phi_1(\rho_i)\right)\otimes
\left(\sum_j q_j\Phi_2(\sigma_j)\right).
$$

The [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) of a tensor product is the sum of its entropies. Applying this both to the average and to every labelled output gives

$$
\chi(\Phi_1\otimes\Phi_2,\mathcal E_1\otimes\mathcal E_2)
=\chi(\Phi_1,\mathcal E_1)+\chi(\Phi_2,\mathcal E_2).
$$

Choose each ensemble within $\varepsilon$ of its supremum. The supremum for the joint channel includes this product ensemble, so its value is at least $\chi^*(\Phi_1)+\chi^*(\Phi_2)-2\varepsilon$. Let $\varepsilon\downarrow0$. The [superadditivity of Holevo capacity](../../../../../../superadditivity-of-holevo-capacity.md) follows:

$$
\boxed{\chi^*(\Phi_1\otimes\Phi_2)\geq\chi^*(\Phi_1)+\chi^*(\Phi_2)}.
$$

This argument does not restrict the joint supremum to product ensembles and does not require the individual suprema to be attained.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
