# Trace and local volume change

↑ **Parent:** [Matrix trace](matrix-trace.md)

For any fixed real $n$-by-$n$ [matrix](matrix.md) $A$, as the real parameter $t$ tends to zero,

$$
\det(I+tA)=1+t\operatorname{tr}A+O(t^2).
$$

The [big O notation](big-o-notation.md) means the remainder is bounded in [absolute value](absolute-value.md) by $Ct^2$ for some constant $C$ near zero. The [determinant](determinant.md) stays positive for sufficiently small $t$, so its [oriented volume](oriented-volume.md) factor is also its ordinary [volume](volume.md) factor. Thus the [trace](matrix-trace.md) is the first-order fractional [volume](volume.md) change, measured from the [identity matrix](identity-matrix.md).

A proof follows directly from [multilinearity of the determinant](multilinearity-of-the-determinant.md). Each column of $I+tA$ is $e_j+tAe_j$. The constant term chooses all the [standard basis](standard-basis.md) columns and equals one. A term containing exactly one factor $t$ replaces just column $j$ by $Ae_j$; expanding that [vector](vector.md) in the [standard basis](standard-basis.md) leaves only its $e_j$ component, $a_{jj}$, because every other choice repeats a column. Summing gives $\operatorname{tr}A$. Terms with two or more replacements have order $t^2$ or higher. This also proves the [derivative of the determinant](derivative-of-the-determinant.md) at the [identity matrix](identity-matrix.md).

This coefficient has a direct visual meaning. At the point $e_j$, the [linear map](linear-map.md) $x\mapsto Ax$ has component $a_{jj}$ along direction $e_j$. In a small step $x\mapsto x+tAx$, these are the first-order changes of the square's or box's sides in their own directions. Summing them gives its fractional [area](surface-area.md) or [volume](volume.md) change; the off-diagonal entries initially change shape rather than contributing to this first-order total.

For the constant-coefficient [linear system of differential equations](linear-system-of-differential-equations.md) $x'=Ax$, the exact [linear flow](linear-flow.md) is $x(t)=e^{tA}x(0)$, using the [matrix exponential](matrix-exponential.md). Its [volume](volume.md) factor is

$$
V(t)=\det(e^{tA})=e^{t\operatorname{tr}A},\qquad V(0)=1,
\qquad V'(t)=(\operatorname{tr}A)V(t).
$$

This is the [matrix exponential determinant identity](matrix-exponential-determinant-identity.md). One can derive it without [diagonalization](diagonalization-of-a-matrix.md): set $E(t)=e^{tA}$, whose [matrix inverse](matrix-inverse-split.md) is $E(-t)$, and use $E'=AE$ in [Jacobi's formula](jacobi-s-formula.md) to get $V'=\det E\operatorname{tr}(E^{-1}AE)=(\operatorname{tr}A)V$. The scalar [differential equation](differential-equation-split.md) with initial value one gives the displayed [exponential function](exponential-function.md). Thus positive [trace](matrix-trace.md) causes [volume](volume.md) expansion, negative [trace](matrix-trace.md) causes contraction, and zero [trace](matrix-trace.md) preserves [volume](volume.md), even when individual directions behave differently.

In two dimensions, compare four generators at $t=0.4$:

$$
\begin{array}{c|c|c|c}
A&\operatorname{tr}A&e^{0.4A}&\text{area factor}\\\hline
\operatorname{diag}(1,1)&2&\operatorname{diag}(e^{0.4},e^{0.4})&e^{0.8}\approx2.2255\\
\operatorname{diag}(1,-1)&0&\operatorname{diag}(e^{0.4},e^{-0.4})&1\\
\operatorname{diag}(-1,-1)&-2&\operatorname{diag}(e^{-0.4},e^{-0.4})&e^{-0.8}\approx0.4493\\
\begin{pmatrix}0&1\\0&0\end{pmatrix}&0&\begin{pmatrix}1&0.4\\0&1\end{pmatrix}&1
\end{array}
$$

The first and third [diagonal matrices](diagonal-matrix.md) expand or contract both directions. The second expands horizontally and contracts vertically by reciprocal factors, making a rectangle of unchanged [area](surface-area.md). For the last [nilpotent matrix](nilpotent-matrix.md), $A^2=0$, so its [matrix exponential](matrix-exponential.md) is exactly $I+tA$; it sends $(x,y)$ to $(x+ty,y)$, a [shear mapping](shear-mapping.md). Zero [trace](matrix-trace.md) allows substantial shape change and does not mean the [flow map](flow-map.md) is stationary.

<a id="image-four-examples-of-a-linear-system-of-differential-equations-trace-controls-area-change-while-a-saddle-and-a-shear-mapping-preserve-area"></a>
![](matrix-trace-local-volume.png)

**[Figure 23](#image-four-examples-of-a-linear-system-of-differential-equations-trace-controls-area-change-while-a-saddle-and-a-shear-mapping-preserve-area). Four examples of a linear system of differential equations: trace controls area change while a saddle and a shear mapping preserve area**.

The first-order statement and the exact [flow map](flow-map.md) should be distinguished. For $A=\operatorname{diag}(1,-1)$, $\det(I+tA)=1-t^2$, whereas $\det(e^{tA})=1$ for all real $t$. Zero [trace](matrix-trace.md) eliminates the first-order change in the approximate step, and it preserves [volume](volume.md) exactly in the [matrix exponential](matrix-exponential.md) flow. The examples use an abstract parameter $t$ and coordinate [vectors](vector.md); no physical units are assumed.

## ↑ Ancestors (6)

1. [Matrix trace](matrix-trace.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Linear flow](linear-flow.md)
- [Matrix trace](matrix-trace.md)
