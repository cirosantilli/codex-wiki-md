<h1 id="26i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For level $k$, let $H_k$ be the horizontal generator: neighboring horizontal sites exchange at rate $1/6$, with reflecting endpoints. It is symmetric and has zero row sums, so the uniform row [vector](../../../../../../vector.md) $u_k=(1/(k+1),\ldots,1/(k+1))$ satisfies $u_kH_k=0$. Removing paths as soon as they jump vertically gives the killed horizontal generator $H_k-(2/3)I$. Therefore

$$
u_ke^{t(H_k-(2/3)I)}=e^{-2t/3}u_k.
$$

Conditional on any elapsed waiting time without a vertical jump, the horizontal position remains uniform. This proves the exit-position uniformity as well as independence of that position from the vertical holding time.

Now consider the upward rate block $U_k$ from level $k$ to $k+1$. For $k>0$ each of its $k+2$ destination columns has sum $1/3$: an endpoint receives its single doubled edge jump, and each other site receives two jumps of rate $1/6$. Hence

$$
(u_kU_k)_j=\frac1{3(k+1)}
=\lambda_k\,\frac1{k+2}.
$$

Likewise every destination column of the downward block $D_k$ has sum $1/3$, so $(u_kD_k)_j=\mu_k/k$. Thus, conditional on either next vertical level, the arrival position is uniform on that new level. At the corner the two upward rates are equal, giving uniform arrival on level one directly.

Starting with the single site at level zero, induction now proves the [uniform conditional law for a triangular-wedge walk](../../../../../../uniform-conditional-law-for-a-triangular-wedge-walk.md): conditional on every attainable past-level sequence, arrival is uniform; the killed semigroup makes departure uniform; and the rate-block column sums make arrival at the following level uniform again. This proves both equalities of the requested property and justifies the averaging in part (b). The statement does not condition departure on the future level, which would in general bias the exit positions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26I](../../26i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
