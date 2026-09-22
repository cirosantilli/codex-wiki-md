<h1 id="40c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Sample the diffusion coefficient at edge midpoints and write

$$
\begin{aligned}
\alpha&=a((i-\tfrac12)h,jh),&
\beta&=a((i+\tfrac12)h,jh),\\
\gamma&=a(ih,(j-\tfrac12)h),&
\delta&=a(ih,(j+\tfrac12)h).
\end{aligned}
$$

Centered differences of the two fluxes give the conservative [finite-difference](../../../../../../../finite-difference-method.md) stencil

$$
\boxed{
\frac1{h^2}\left[
\alpha u_{i-1,j}+\beta u_{i+1,j}
+\gamma u_{i,j-1}+\delta u_{i,j+1}
-(\alpha+\beta+\gamma+\delta)u_{i,j}
\right]}.
$$

For example, the $x$ part is

$$
\frac1h\left[
a_{i+1/2,j}\frac{u_{i+1,j}-u_{i,j}}h
-a_{i-1/2,j}\frac{u_{i,j}-u_{i-1,j}}h
\right].
$$

Taylor expansion about $(ih,jh)$ shows that the odd powers cancel between the two face fluxes and that the result equals $\partial_x(a\,u_x)+O(h^2)$. The same calculation in $y$ gives total truncation error

$$
\boxed{O(h^2)}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [40C](../../../40c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
