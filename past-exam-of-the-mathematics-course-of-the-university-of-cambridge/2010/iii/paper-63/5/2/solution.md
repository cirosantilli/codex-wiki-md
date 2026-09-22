<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $\delta=\Delta t$ and $L=A+B$, keeping the spatial grid fixed for the temporal error assertion. The [matrix exponential](../../../../../../matrix-exponential.md) expansions give

$$
S_\delta:=e^{\delta A}e^{\delta B}
=I+\delta L+\delta^2(\tfrac12A^2+AB+\tfrac12B^2)+O(\delta^3),
$$



$$
E_\delta:=e^{\delta L}=I+\delta L+\tfrac12\delta^2(A^2+AB+BA+B^2)+O(\delta^3).
$$

Hence the [Lie-Trotter splitting commutator error](../../../../../../lie-trotter-splitting-commutator-error.md) is

$$
S_\delta-E_\delta=\tfrac12\delta^2[A,B]+O(\delta^3).
$$

The energy estimate from part 1 makes $e^{tA}$, $e^{tB}$ and $e^{tL}$ contractions, so both $S_\delta$ and $E_\delta$ have norm at most one. Telescope their $n$th powers:

$$
S_\delta^n-E_\delta^n
=\sum_{j=0}^{n-1}S_\delta^{n-1-j}(S_\delta-E_\delta)E_\delta^j.
$$

For $n\delta\le T$, this gives

$$
\boxed{\|S_\delta^nu^0-e^{n\delta L}u^0\|_h
\le nC_h\delta^2\|u^0\|_h\le C_hT\delta\|u^0\|_h.}
$$

Thus the [Lie-Trotter splitting](../../../../../../lie-product-formula.md) has global temporal error $O(\Delta t)$. The constant here may depend on the fixed spatial operators; a mesh-uniform joint-limit error estimate needs additional regularity and [commutator](../../../../../../commutator.md) bounds. If $A$ and $B$ commute, this particular exponential splitting is exact, but variable diffusion coefficients generally remove that commutativity.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
