<h1 id="23k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the neutral [Moran model](../../../../../../moran-process.md), a fixed population of $N$ individuals carries either allele $a$ or its alternative. Each individual reproduces at rate one and replaces a uniformly selected individual. If $i$ carry $a$, the two changing-state rates are $q_{i,i+1}=q_{i,i-1}=i(N-i)/N$. States zero and $N$ are absorbing. This time normalization is essential for the stated expected time.

The hitting probability $h_i$ of $N$ before zero satisfies $h_{i+1}-2h_i+h_{i-1}=0$, with $h_0=0,h_N=1$. Thus $\boxed{h_i=i/N}$. Let $G_{ij}$ be expected occupation time at $j$ before absorption. The [Green function](../../../../../../green-s-function.md) equation in its starting index is

$$
\frac{i(N-i)}N(G_{i+1,j}-2G_{ij}+G_{i-1,j})=-\mathbf1_{\{i=j\}},\qquad G_{0j}=G_{Nj}=0.
$$

It is linear on either side of $j$. Matching values and the difference jump at $j$ gives

$$
G_{ij}=\begin{cases}i/j,&i\leq j,\\(N-i)/(N-j),&i\geq j.\end{cases}
$$

For example the difference jump is $-N/[j(N-j)]$, so multiplying by $j(N-j)/N$ gives exactly $-1$.

Condition on fixation using part (i), with $A=\{N\}$ and the occupation stopped on absorption at either endpoint; on paths absorbed at zero, hitting $N$ is impossible. Equivalently apply the Markov-property occupation proof directly to this event. The conditional occupation time at $j$ is $(j/i)G_{ij}$. For $j\geq i$ it is one; for $j<i$ it is $[(N-i)/i]j/(N-j)$. Summing over all transient states yields

$$
\boxed{\mathbb E_i[\tau\mid\text{fixation}]=N-i+\frac{N-i}{i}\sum_{j=1}^{i-1}\frac{j}{N-j}.}
$$

Here $1\leq i\leq N$; at $i=N$ the fixation time is zero, while at $i=0$ conditioning is undefined.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [23K](../../23k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
