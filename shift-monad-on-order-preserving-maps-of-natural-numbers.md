# Shift monad on order-preserving maps of natural numbers

↑ **Parent:** [Monad](monad.md)

Let $M$ be the [monoid](monoid.md) of [order-preserving functions](order-preserving-function.md) $\mathbb N\to\mathbb N$, with $\mathbb N=\{0,1,\ldots\}$, regarded as a one-object [category](category-split.md). The endofunctor $T$ fixes that object and sends $f$ to $Tf(0)=0$, $Tf(n+1)=f(n)+1$. The displayed maps give its [monad](monad.md) unit and multiplication. The multiplication is not injective, so this is not an [idempotent monad](idempotent-monad.md). Its only [algebra for a monad](algebra-for-a-monad.md) is $\mu$, because $a\eta=1$ forces $a(n+1)=n$ and monotonicity forces $a(0)=0$. Algebra endomorphisms are exactly the functions fixing zero. The [Kleisli comparison functor](kleisli-comparison-functor.md) sends $f$ to the function which is zero at zero and equals $f(n)$ at $n+1$; its inverse sends $h$ to $n\mapsto h(n+1)$. Thus the comparison is an isomorphism of categories even though the monad is not idempotent.

## ↑ Ancestors (6)

1. [Monad](monad.md)
2. [Category theory](category-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119/4/iii/solution.md)
