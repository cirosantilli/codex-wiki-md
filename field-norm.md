# Field norm

↑ **Parent:** [Algebraic number theory](algebraic-number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Field_norm)

For a [finite field extension](finite-field-extension.md) $L/K$, multiplication by $\alpha\in L$ is a $K$-[linear map](linear-map.md) $m_\alpha:L\to L$. Its [determinant](determinant.md) is the field norm:

$$
N_{L/K}(\alpha)=\det(m_\alpha)\in K.
$$

This does not depend on the chosen [basis](basis.md). If $L/K$ is a [separable field extension](separable-extension.md), then

$$
N_{L/K}(\alpha)=\prod_{\sigma:L\hookrightarrow\overline K,\ \sigma|_K=\operatorname{id}}\sigma(\alpha),
$$

where the product runs over all $[L:K]$ [field embeddings](field-embedding.md) into an [algebraic closure](algebraic-closure.md) of $K$. Embeddings are counted even when several give the same value on $\alpha$: for $r\in K$, the result is $r^{[L:K]}$. This avoids ambiguity in the phrase “product of [algebraic conjugates](conjugate-element-field-theory.md)”.[Andrew Sutherland, Number Theory I, Lecture 4, norm and trace](https://math.mit.edu/classes/18.785/2021fa/LectureNotes4.pdf)

For $L=\mathbb Q(\sqrt2)$ over $K=\mathbb Q$, write $\alpha=a+b\sqrt2$. In the [basis](basis.md) $1,\sqrt2$, multiplication by $\alpha$ has columns $(a,b)$ and $(2b,a)$, hence

$$
M_\alpha=\begin{pmatrix}a&2b\\b&a\end{pmatrix},\qquad
N_{L/\mathbb Q}(\alpha)=a^2-2b^2=(a+b\sqrt2)(a-b\sqrt2).
$$

The [determinant](determinant.md) calculation and the product of the two [field embeddings](field-embedding.md) give the same answer. In particular,

$$
N(\sqrt2)=-2,\qquad N(1+\sqrt2)=-1,\qquad N(3+2\sqrt2)=1,\qquad N(2)=4.
$$

A [field norm](field-norm.md) is an arithmetic invariant; it is not a nonnegative [norm](norm.md) measuring length, and need not be positive on nonzero elements.

The [field norm](field-norm.md) is multiplicative, $N(\alpha\beta)=N(\alpha)N(\beta)$, because $m_{\alpha\beta}=m_\alpha m_\beta$ and [determinants](determinant.md) are multiplicative. It vanishes exactly at zero. For a [number field](number-field.md) over $\mathbb Q$, it takes [algebraic integers](algebraic-integer.md) to [integers](integer.md), and an [algebraic integer](algebraic-integer.md) is a [unit](unit-in-a-ring.md) exactly when its [field norm](field-norm.md) is $1$ or $-1$.[Sutherland, Lecture 4, properties of the norm](https://math.mit.edu/classes/18.785/2021fa/LectureNotes4.pdf)[Conrad, Quadratic Integers, norms and units in quadratic rings](https://kconrad.math.uconn.edu/blurbs/ugradnumthy/quadratic-integers.pdf)

This makes the [field norm](field-norm.md) a useful test for [divisibility](divisibility.md). If nonzero $\alpha,\beta\in\mathcal O_L$ and $\alpha$ divides $\beta$, then the [integer](integer.md) $N(\alpha)$ divides $N(\beta)$. For example, $3+\sqrt2$ has [field norm](field-norm.md) $7$, so it cannot divide $2$, whose [field norm](field-norm.md) is $4$. It does divide $7$, with quotient $3-\sqrt2$. This necessary condition can reject a proposed factor without solving for its quotient.

**Table of contents**

- [Norm of an integral element over a normal domain](norm-of-an-integral-element-over-a-normal-domain.md)
- [Unit norm detects units in a local extension](unit-norm-detects-units-in-a-local-extension.md)
- [Norm form](norm-form.md)
  - [Prime representation by the norm form of Q of square root 229](prime-representation-by-the-norm-form-of-q-of-square-root-229.md)
- [Norm obstruction to being a square](norm-obstruction-to-being-a-square.md)
- [Unit from norm one or minus one](unit-from-norm-one-or-minus-one.md)

## ↑ Ancestors (5)

1. [Algebraic number theory](algebraic-number-theory-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (73)

- [Algebraic number theory](algebraic-number-theory-split.md)
- [Brauer class](brauer-class.md)
- [Cyclotomic Euler norm factor at a new prime](cyclotomic-euler-norm-factor-at-a-new-prime.md)
- [Discreteness of principal ideles](discreteness-of-principal-ideles.md)
- [Effective norm-form height estimate](effective-norm-form-height-estimate.md)
- [Explicit quadratic Hilbert symbols over the p-adic numbers](explicit-quadratic-hilbert-symbols-over-the-p-adic-numbers.md)
- [Field norm](field-norm.md)
- [Finite extension stability of C1 fields](finite-extension-stability-of-c1-fields.md)
- [Hasse norm theorem](hasse-norm-theorem.md)
- [Ideal class group of Q of square root 229](ideal-class-group-of-q-of-square-root-229.md)
- [Ideal class group of Q square root of minus fourteen](ideal-class-group-of-q-square-root-of-minus-fourteen.md)
- [Norm-compatible sequence of local units](norm-compatible-sequence-of-local-units.md)
- [Norm detects proper closed subsets under finite normalization](norm-detects-proper-closed-subsets-under-finite-normalization.md)
- [Norm-Euclideanity of the integers adjoined square root two](norm-euclideanity-of-the-integers-adjoined-square-root-two.md)
- [Norm for a finite free ring extension](norm-for-a-finite-free-ring-extension.md)
- [Norm projection formula for cyclic Brauer pairings](norm-projection-formula-for-cyclic-brauer-pairings.md)
- [Norm subgroup of a local field extension](norm-subgroup-of-a-local-field-extension.md)
- [Normalized local factors for the product formula](normalized-local-factors-for-the-product-formula.md)
- [Number field](number-field.md)
- [Orthonormalization of a finite-field Hermitian form](orthonormalization-of-a-finite-field-hermitian-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-74/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-15/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-23/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-23/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-23/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-27/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/20g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/11h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/11h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/18g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-31/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-31/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-4/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-4/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/20g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/20g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-26/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/20g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/20g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-32/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-28/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/18h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-21/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-21/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-21/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-21/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-24/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/16h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/11e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/18h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/19h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/20g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/20g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/20h/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-136/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/18h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-166/2/b/solution.md)
- [Quadratic finite-field norm and trace surjectivity](quadratic-finite-field-norm-and-trace-surjectivity.md)
- [Ring of integers of a quadratic field](ring-of-integers-of-a-quadratic-field.md)
- [Ring of integers of Q of square root two](ring-of-integers-of-q-of-square-root-two.md)
- [Surjectivity of unit norms in unramified extensions](surjectivity-of-unit-norms-in-unramified-extensions.md)
- [Unit form of Hilbert theorem 90](unit-form-of-hilbert-theorem-90.md)
- [Unit from norm one or minus one](unit-from-norm-one-or-minus-one.md)
- [Unit norm detects units in a local extension](unit-norm-detects-units-in-a-local-extension.md)
- [Units of Q of square root two](units-of-q-of-square-root-two.md)
