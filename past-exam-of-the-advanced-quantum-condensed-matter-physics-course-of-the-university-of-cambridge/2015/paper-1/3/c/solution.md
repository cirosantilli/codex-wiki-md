<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix canonical single-particle order $(1\uparrow,1\downarrow,2\uparrow,2\downarrow)$ and write the occupation ket as $|n_1n_2n_3n_4\rangle$. The six states in the printed order are $|1010\rangle$, $|1001\rangle$, $|0110\rangle$, $|0101\rangle$, $|1100\rangle$, $|0011\rangle$. The last state is [double occupancy](../../../../../double-occupancy.md) on site 2.

For a [fermionic raising and lowering operator](../../../../../fermionic-raising-and-lowering-operator.md) acting on mode $j$, the sign is $(-1)^{\sum_{k<j}n_k}$, and annihilation requires that mode occupied while creation requires it empty. Starting from the second basis state, the hop that reaches the last state is

$$
c_{2\uparrow}^\dagger c_{1\uparrow}|1001\rangle
=c_{2\uparrow}^\dagger|0001\rangle=|0011\rangle.
$$

It therefore contributes **$H_{6,2}=-t$**. Starting from the third state instead,

$$
c_{2\downarrow}^\dagger c_{1\downarrow}|0110\rangle
=c_{2\downarrow}^\dagger|0010\rangle=-|0011\rangle,
$$

because the occupied $2\uparrow$ mode precedes $2\downarrow$. The [Hamiltonian](../../../../../hamiltonian.md)'s leading $-t$ makes **$H_{6,3}=+t$**. Finally $n_{2\uparrow}n_{2\downarrow}|0011\rangle=|0011\rangle$, so **$H_{6,6}=U$**. No other displayed basis state reaches $|0011\rangle$ in one allowed hop. These signs verify the three nonzero entries without assigning distinguishable-particle hopping signs to fermions.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
