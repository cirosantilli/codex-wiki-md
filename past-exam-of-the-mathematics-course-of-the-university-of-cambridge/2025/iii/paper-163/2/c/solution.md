<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take all coefficients equal to one, so $\sum|b_n|^2\asymp N^2$. At each $t_0\in\mathcal T$, parts a and b, with the negligible tail absorbed, give

$$
\int_{B_{t_0}}|f(x,t)|\,dxdt\gtrsim N^{-2}.
$$

The box has volume $\asymp N^{-4+3\epsilon}$. Hölder's inequality therefore yields

$$
\int_{B_{t_0}}|f|^p
\gtrsim N^{-2p}N^{(4-3\epsilon)(p-1)}
=N^{2p-4-O_p(\epsilon)}.
$$

The time boxes are disjoint because the selected times are one-separated. Summing over $|\mathcal T|\gtrsim T/N^2$ gives

$$
\int_{[0,1]^2\times[0,T]}|f|^p
\gtrsim T N^{2p-6-O_p(\epsilon)}.
$$

Dividing by $(\sum|b_n|^2)^{p/2}\asymp N^p$ and renaming the epsilon loss proves

$$
D_p(N,T)\gtrsim_\epsilon N^{-\epsilon}TN^{p-6}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 163](../../../paper-163-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
