<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose the angle register stores a fixed-point expansion $\theta_i=\sum_{r=1}^q\theta_{ir}2^{-r}\theta_{\max}$. Append a target qubit in $|0\rangle$. For each angle bit $	heta_{ir}$, apply to the target a controlled $R_y(2^{1-r}\theta_{\max})$. Rotations about the same axis commute, so their product is $R_y(2\theta_i)$ and

$$
|0\rangle\longmapsto
\cos\theta_i|0\rangle+\sin\theta_i|1\rangle.
$$

With $q=O(\operatorname{poly}\log N)$ retained bits, each controlled rotation decomposes into one- and two-qubit gates and the complete [quantum variable rotation](../../../../../../../quantum-variable-rotation.md) has polylogarithmic size. Thus the required branchwise map is implemented coherently for every $i$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
