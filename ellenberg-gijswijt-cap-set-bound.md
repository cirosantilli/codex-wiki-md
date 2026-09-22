<h1 id="ellenberg-gijswijt-cap-set-bound">Ellenberg–Gijswijt cap-set bound</h1>

↑ **Parent:** [Cap set](cap-set.md)

There is a constant $C<3$ such that every [cap set](cap-set.md) in $\mathbb F_3^n$ has cardinality less than $C^n$.

For the [polynomial method in combinatorics](polynomial-method-in-combinatorics.md), use

$$
T(x,y,z)=\prod_{i=1}^n\bigl(1-(x_i+y_i+z_i)^2\bigr).
$$

Over $\mathbb F_3$, this is the [indicator function](indicator-function.md) of $x+y+z=0$. On $A^3$ it is therefore a diagonal tensor with $|A|$ nonzero diagonal entries. Every [monomial](monomial.md) in its expansion has individual exponents at most two and total degree at most $2n$, so one of its three variable blocks has degree at most $2n/3$. Grouping terms according to such a block and using the [slice rank of a diagonal tensor](slice-rank-of-a-diagonal-tensor.md) gives

$$
|A|=\operatorname{slice\ rank}(T|_{A^3})\leq3m_n,
$$

where $m_n$ is the number of $\alpha\in\{0,1,2\}^n$ with $\sum_i\alpha_i\leq2n/3$. If $X_i=1-\alpha_i$ are [independent random variables](independent-random-variables.md) uniform on $\{-1,0,1\}$, then

$$
\frac{m_n}{3^n}=\mathbb P\left(\sum_iX_i\geq\frac n3\right).
$$

Any exponential upper bound for this [tail probability](tail-probability.md) gives $m_n\leq(3-\epsilon)^n$ and hence the result after absorbing the factor three and finitely many small dimensions into $C<3$.

**Table of contents**

- [Low-degree monomial count for the cap-set bound](low-degree-monomial-count-for-the-cap-set-bound.md)

## ↑ Ancestors (6)

1. [Cap set](cap-set.md)
2. [Polynomial method in combinatorics](polynomial-method-in-combinatorics.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Meshulam bound for cap sets](meshulam-bound-for-cap-sets.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/3/solution.md)
