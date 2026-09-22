<h1 id="20h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $F:|K|\times[0,1]\to|L|$ be a [homotopy](../../../../../../homotopy.md) from $f$ to $g$. The inverse images $F^{-1}(\operatorname{st}_L(w))$ form a finite open cover of the compact product. By the [Lebesgue number lemma](../../../../../../lebesgue-number-lemma.md) there is $\delta>0$ such that every subset of diameter less than $\delta$ lies in one of these inverse images.

Choose a [barycentric subdivision](../../../../../../barycentric-subdivision.md) $K^{(n)}$ with all its open stars of diameter less than $\delta/3$, and times $0=t_0<\cdots<t_m=1$ with gaps less than $\delta/6$. For each vertex $v$ and each time $t_i$, the set

$$
\operatorname{st}(v)\times J_i,\qquad J_i=[t_{i-1},t_{i+1}]\cap[0,1]
$$

(with the evident endpoint conventions) has diameter less than $\delta$ in the product metric. Choose a vertex $w_i(v)$ of $L$ whose open star contains its image under $F$, and set $h_i(v)=w_i(v)$.

At time $t_i$, the star condition makes $h_i$ a simplicial approximation to $F(\cdot,t_i)$. Adjacent intervals $J_i,J_{i+1}$ overlap, so choose a time in their overlap and a point in the interior of any simplex $\sigma$ of $K^{(n)}$. Its image belongs to the stars of every $h_i(v)$ and $h_{i+1}(v)$ for $v\in\sigma$. As in (i), their vertices lie in one carrier simplex, proving contiguity. Thus the sequence starts with an approximation to $f$, ends with one to $g$, and has contiguous adjacent pairs. Relabeling its indices gives the requested $h_1,\ldots,h_m$.

Here $\sim_c$ denotes contiguity, with the endpoint maps approximating $f,g$ respectively.

$$
\boxed{f\simeq g\ \Longrightarrow\ h_1\sim_c h_2\sim_c\cdots\sim_c h_m\text{ on some }K^{(n)}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
