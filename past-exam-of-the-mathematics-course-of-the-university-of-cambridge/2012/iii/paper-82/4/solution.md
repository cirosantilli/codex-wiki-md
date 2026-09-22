<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the uniform [probability measure](../../../../../probability-measure.md) on the [Boolean hypercube](../../../../../boolean-hypercube.md). The [influence of a variable](../../../../../influence-of-a-variable.md) is the flip [probability](../../../../../probability.md)

$$
I_i(f)=\mathbb P(f(x)\ne f(x+e_i)).
$$

The [polynomial](../../../../../polynomial-split.md) defining $f$ is interpreted over $\mathbb F_2$. Flipping the first coordinate adds $x_2+\cdots+x_n$ modulo two. This nonempty parity is balanced for $n\ge2$, so

$$
\boxed{I_1(f)=1/2.}
$$

An explicit [Tribes function](../../../../../tribes-function.md) works for every $n\ge2$. Choose the largest integer $w\ge1$ with $w2^w\le n$, let $m=\lfloor2^w\log2\rfloor$, and take the OR of $m$ disjoint ANDs of $w$ coordinates. Ignore the unused coordinates. Its zero [probability](../../../../../probability.md) is $(1-2^{-w})^m$, between $1/4$ and $3/4$, and a used coordinate has [influence](../../../../../influence-of-a-variable.md)

$$
2^{-(w-1)}(1-2^{-w})^{m-1}\le2^{1-w}<\frac{4(w+1)}n\le\frac{12\log n}{n}<\frac{100\log n}{n}.
$$

Here $n<2^{w+1}(w+1)$ by maximality. For the balance claim, $w=1$ gives [probability](../../../../../probability.md) $1/2$; for $w\ge2$, $m\ge2^w\log2-1$ gives zero [probability](../../../../../probability.md) at most $e^{-\log2+2^{-w}}<3/4$, while $(1-1/q)^q\ge1/4$ for $q=2^w\ge2$ gives a lower bound $(1/4)^{\log2}>1/4$. Only the example was requested, but these checks fix its parameters unambiguously.

For the lower bound we prove the required consequence of [Beckner's inequality](../../../../../beckner-s-inequality.md) with constants. Write the [Fourier-Walsh transform](../../../../../fourier-walsh-transform.md) as $f=\sum_S\widehat f(S)\chi_S$, where $\chi_S(x)=(-1)^{\sum_{i\in S}x_i}$ and $\widehat f(S)=\mathbb E(f\chi_S)$. The [discrete derivative of a Boolean function](../../../../../discrete-derivative-of-a-boolean-function.md) is $D_if=(f-f(\cdot+e_i))/2$. Since $f$ takes values zero and one, $D_if$ takes values $0,\pm1/2$. Consequently [Parseval's identity](../../../../../parseval-identity.md) gives

$$
I_i(f)=4\sum_{S\ni i}|\widehat f(S)|^2,
\qquad I:=\sum_iI_i(f)=4\sum_S|S|\,|\widehat f(S)|^2.
$$

**The factor four is required for the printed $0/1$ convention.** Also $V:=\operatorname{Var}(f)=\sum_{S\ne\varnothing}|\widehat f(S)|^2\ge3/16$ under the balance hypothesis.

The true [Beckner's inequality](../../../../../beckner-s-inequality.md) states $\|T_\rho h\|_q\le\|h\|_p$ for $1<p\le q<\infty$, $0\le\rho\le\sqrt{(p-1)/(q-1)}$, with $T_\rho h=\sum_S\rho^{|S|}\widehat h(S)\chi_S$. Apply it with $p=3/2$, $q=2$, $\rho=1/\sqrt2$ to $h_i=\chi_{\{i\}}D_if$, a [function](../../../../../function-split.md) independent of coordinate $i$. Its nonzero values still have magnitude $1/2$. We obtain

$$
\sum_{S\ni i}2^{-(|S|-1)}|\widehat f(S)|^2
\le\|h_i\|_{3/2}^2=\frac14 I_i(f)^{4/3}.
$$

Let $a=\max_iI_i(f)>0$. For an integer $\ell\ge1$, the low-degree [Fourier weight](../../../../../fourier-weight.md) satisfies

$$
\sum_{1\le|S|\le\ell}|\widehat f(S)|^2
\le\sum_{1\le|S|\le\ell}|S|\,|\widehat f(S)|^2
\le\frac{2^{\ell-1}}4\sum_iI_i^{4/3}\le\frac{2^{\ell-1}}4na^{4/3}.
$$

For the high-degree part the [total influence](../../../../../total-influence.md) identity gives

$$
\sum_{|S|>\ell}|\widehat f(S)|^2\le\frac{I}{4(\ell+1)}\le\frac{na}{4(\ell+1)}.
$$

Together these imply $4V\le na\bigl(2^{\ell-1}a^{1/3}+1/(\ell+1)\bigr)$.

Suppose, seeking a contradiction, that $a<\log n/(100n)$, with natural logarithms. Then $a<1/(100e)$ and $\ell=\lfloor\log(1/a)/(6\log2)\rfloor\ge1$. Hence $2^{\ell-1}a^{1/3}\le a^{1/6}/2$. Put $y=\log n$. The first term on the right is bounded by

$$
\frac n2a^{7/6}\le\frac{y^{7/6}e^{-y/6}}{2\cdot100^{7/6}}
\le\frac{7^{7/6}e^{-7/6}}{2\cdot100^{7/6}}<\frac1{100};
$$

the middle expression is maximized at $y=7$. Moreover $\log(1/a)\ge y/2$, since $y\le100e^{y/2}$. Thus

$$
\frac{na}{\ell+1}\le\frac{6\log2\,na}{\log(1/a)}\le\frac{12\log2}{100}<\frac9{100}.
$$

We would have $4V<1/10$, contradicting $4V\ge3/4$. Therefore

$$
\boxed{\max_{1\le i\le n}I_i(f)\ge\frac{\log n}{100n}.}
$$

This derives the stated [Kahn-Kalai-Linial theorem](../../../../../kahn-kalai-linial-theorem.md) bound from the actual [noise operator on the Boolean hypercube](../../../../../noise-operator-on-the-boolean-hypercube.md) inequality, rather than using the desired conclusion as an input.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [Section B](../section-b.md)
3. [Paper 82](../../paper-82-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
