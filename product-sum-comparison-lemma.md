# Product-sum comparison lemma

↑ **Parent:** [Cardinal arithmetic](cardinal-arithmetic.md)

In ZF, let $K,L$ be nonempty. If $K\times L$ injects into $K\sqcup L$, then there is either an injection or a surjection from $K$ to $L$.

Indeed, extend the inverse of the given injection to a surjection $p:K\sqcup L\to K\times L$ by sending points outside its range to one fixed pair $(k_*,l_*)$. If the second coordinate of $p$ restricted to the $K$-summand covers $L$, it is the required surjection. Otherwise choose $l_0$ that it misses. Every $(k,l_0)$ then has its preimage in the $L$-summand. Except possibly for the default pair, that preimage is unique, so these preimages inject $K$ into $L$. In the exceptional case they inject $K\setminus\{k_*\}$ into $L$; either their image is all of $L$, yielding a surjection from $K$, or an omitted point extends the map to an injection from $K$.

## ↑ Ancestors (7)

1. [Cardinal arithmetic](cardinal-arithmetic.md)
2. [Cardinal number](cardinal-number.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/16h/c/solution.md)
- [Tarski cardinal-square theorem](tarski-cardinal-square-theorem.md)
