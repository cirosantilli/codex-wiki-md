<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [free monoid](../../../../../../free-monoid.md) on $x,y$, use the function

$$
f(w,n)=\begin{cases}
1,&|w|>n\text{ and the final letter of }w\text{ is }x,\\
0,&\text{otherwise}.
\end{cases}
$$

The strict inequality is important. For any prefix $v$, $|vw|>|v|+n$ is equivalent to $|w|>n$. Whenever it holds, $w$ is nonempty and prefixing $v$ does not change its final letter. When it fails, both values are zero. Thus

$$
f(vw,n+|v|)=f(w,n),
$$

which proves equivariance for the diagonal action on $M\times\mathbb N$ and the trivial action on $B$. Hence $f$ is an element of the exponential described above. Let $g$ be the constant-zero equivariant function. They differ at $(x,0)$.

But every word $wy$ ends in $y$, so

$$
(y\cdot f)(w,n)=f(wy,n)=0=(y\cdot g)(w,n)
$$

for every $w,n$. The action of $y$ on $B^A$ is not injective, and **$B^A$ is not decidable**, even though $B$ is decidable. This is a [nondecidable exponential of decidable monoid sets](../../../../../../nondecidable-exponential-of-decidable-monoid-sets.md). The [monoid](../../../../../../monoid.md) condition in part (a) also fails here: $|pmq|=|p|+|m|+|q|$ cannot equal $|p|$ for a nonempty word $m$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
