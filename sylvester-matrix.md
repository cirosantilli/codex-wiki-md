# Sylvester matrix

↑ **Parent:** [Resultant](resultant.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylvester_matrix)

For [polynomials](polynomial-split.md) $f,g$ of [polynomial degrees](degree-of-a-polynomial.md) $m,n$, the [Sylvester matrix](sylvester-matrix.md) has $n$ shifted coefficient rows of $f$ followed by $m$ shifted rows of $g$, using descending-power order. It is a square [matrix](matrix.md) of size $m+n$. Its [transpose](transpose.md) represents the [linear map](linear-map.md) $(A,B)\mapsto Af+Bg$ with $\deg A<n$, $\deg B<m$; its [determinant](determinant.md) is the [resultant](resultant.md).

For an original parameter example, choose $f(x)=x^2-1$ and $g_t(x)=x-t$. Then

$$
S(f,g_t)=\begin{pmatrix}1&0&-1\\1&-t&0\\0&1&-t\end{pmatrix},\qquad
\operatorname{Res}_x(f,g_t)=t^2-1.
$$

The two lists of [coefficients](coefficient.md) become three rows because $g_t$ is multiplied by both $x$ and $1$. Thus **the common-root parameter values are $t=-1$ and $t=1$**. At $t=1/2$, the [resultant](resultant.md) is $-3/4$, so the two [polynomials](polynomial-split.md) have no [common root](common-root.md).

<a id="image-a-sylvester-matrix-tests-when-a-moving-root-of-a-polynomial-coincides-with-a-fixed-one"></a>
![](resultant-root-test-and-parameter.png)

**[Figure 7](#image-a-sylvester-matrix-tests-when-a-moving-root-of-a-polynomial-coincides-with-a-fixed-one). A Sylvester matrix tests when a moving root of a polynomial coincides with a fixed one**. Original example $f(x)=x^2-1$, $g_t(x)=x-t$. Left: the vertical dashed line marks the [root of a polynomial](root-of-a-polynomial.md) of $g_{1/2}$; it does not make $f$ zero. Right: the same test for all parameters is the [function graph](graph-of-a-function.md) of the [resultant](resultant.md) $t^2-1$. A crossing between two arbitrary function curves would not suffice: both values must be zero.

One can verify the certificate without any [determinant](determinant.md) expansion:

$$
f(x)-(x+t)g_t(x)=t^2-1.
$$

For $t\ne\pm1$, division by $t^2-1$ gives a [Bézout's identity for polynomials](bezout-s-identity-for-polynomials.md). At $t=1$, the identity instead becomes a nontrivial cancellation between multiples of two [polynomials](polynomial-split.md) sharing the [polynomial factor](polynomial-factor.md) $x-1$.

The general proof needs only a short [linear algebra](linear-algebra-split.md) outline. A [common polynomial factor](common-polynomial-factor.md) gives a nonzero cancelling pair $Af+Bg=0$ within the degree bounds, making the [Sylvester matrix](sylvester-matrix.md) singular. Conversely, if $f,g$ are [coprime polynomials](coprime-polynomials.md) and $Af=-Bg$, then $f$ divides $B$; the bound $\deg B<m$ forces $B=0$ and then $A=0$. Thus the [linear map](linear-map.md) has zero [kernel of a linear map](kernel-of-a-linear-map-split.md) exactly in the coprime case. Over an [algebraic closure](algebraic-closure.md), a nonconstant [common polynomial factor](common-polynomial-factor.md) is equivalent to a [common root](common-root.md).

In 1840, [James Joseph Sylvester](james-joseph-sylvester.md) described forming the shifted coefficient rows and taking a signed sum of products selected by [permutations](permutation.md). In modern notation, this is the [Sylvester matrix](sylvester-matrix.md) and its [determinant](determinant.md). The construction turns the nonlinear common-[root of a polynomial](root-of-a-polynomial.md) question into [linear algebra](linear-algebra-split.md). His paper's word _derivatives_ concerns elimination, rather than the [formal derivative](formal-derivative.md) used below.[The Collected Mathematical Papers of James Joseph Sylvester, Volume I; Paper 9, A method of determining by mere inspection the derivatives from two equations of any degree; Collected Mathematical Papers, volume I (1904), pp. 54–55, rules 1–4; original Philosophical Magazine XVI (1840), pp. 132–135](the-collected-mathematical-papers-of-james-joseph-sylvester-volume-i/a-method-of-determining-by-mere-inspection-the-derivatives-from-two-equations-of-any-degree.md)

## ↑ Ancestors (6)

1. [Resultant](resultant.md)
2. [Polynomial](polynomial-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Degree drop in a specialized resultant](degree-drop-in-a-specialized-resultant.md)
- [Eliminating a variable with a resultant](eliminating-a-variable-with-a-resultant.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8/2/solution.md)
- [Resultant](resultant.md)
- [Sylvester matrix](sylvester-matrix.md)
