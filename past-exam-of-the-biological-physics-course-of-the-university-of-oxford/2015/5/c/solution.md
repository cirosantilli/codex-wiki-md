<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret the irreversible limit as a large favorable drop for **each forward step**, so backward transitions during the observation can be neglected. Let the distinct forward rates be $k_1,k_2>0$. The first waiting time has [probability density](../../../../probability-density.md) $k_1e^{-k_1t_1}$; conditional on its completion, the second has independent [probability density](../../../../probability-density.md) $k_2e^{-k_2(t-t_1)}$. Integrating over the first completion time gives the [convolution](../../../../convolution.md)

$$
p_{1,2}(t)=\int_0^t k_1e^{-k_1t_1}k_2e^{-k_2(t-t_1)}\,dt_1
=\frac{k_1k_2}{k_2-k_1}\left(e^{-k_1t}-e^{-k_2t}\right),\quad t\ge0.
$$

Hence

$$
\boxed{\Pr(t<T_1+T_2<t+dt)=p_{1,2}(t)\,dt+o(dt).}
$$

The expression is symmetric under interchanging the rates, positive for either ordering, and integrates to one. Reverse rate constants do not enter this approximation; merely making all four constants different would not justify eliminating them without the downhill condition.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
