<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T=\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$ and $S=\left(\begin{smallmatrix}0&-1\\1&0\end{smallmatrix}\right)$. For $\gamma=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$ in the [modular group](../../../../../../modular-group.md), left multiplication by powers of $T$ and by $S$ performs subtraction and exchange on its first-column entries. The [Euclidean algorithm](../../../../../../euclidean-algorithm.md) reduces $(a,c)$ to $(\pm1,0)$, since the [determinant](../../../../../../determinant.md) condition makes them coprime. The resulting matrix is $\pm T^m$, and $-I=S^2$ is already generated. Hence $S,T$ generate $SL_2(\mathbb Z)$.

The [standard fundamental domain of the modular group](../../../../../../standard-fundamental-domain-of-the-modular-group.md) is $D=\{z\in\mathbb H:|\operatorname{Re}z|\le1/2,\ |z|\ge1\}$, with the vertical sides identified by $T$ and the circular sides by $S$. To prove every orbit meets it, choose a coprime integer pair $(c,d)$ minimizing $|cz+d|$. A minimum exists because only finitely many pairs have this quantity below any fixed bound: $|c|\operatorname{Im}z\le|cz+d|$ bounds $c$, then $d$. Complete the pair to a determinant-one matrix. Its image has maximal imaginary part in the orbit, since $\operatorname{Im}(\gamma z)=\operatorname{Im}z/|cz+d|^2$. Translate its real part into $[-1/2,1/2]$. If its modulus were below one, inversion would increase its imaginary part, a contradiction. This is the [reduction to the standard modular region](../../../../../../reduction-to-the-standard-modular-region.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
