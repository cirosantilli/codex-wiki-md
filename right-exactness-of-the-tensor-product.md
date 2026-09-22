# Right exactness of the tensor product

↑ **Parent:** [Tensor product of modules](tensor-product-of-modules.md)

For a [short exact sequence](short-exact-sequence.md) $0\to U\xrightarrow{i}V\xrightarrow{q}W\to0$ and any [module](module-mathematics.md) $E$, the sequence $U\otimes_AE\to V\otimes_AE\to W\otimes_AE\to0$ is exact. The last map is surjective since every pure tensor $w\otimes e$ can be lifted using a preimage of $w$. Put $T=(V\otimes_AE)/\operatorname{im}(i\otimes1_E)$. There is a well-defined balanced map $W\times E\to T$, sending $(q(v),e)$ to the class of $v\otimes e$: replacing $v$ by $v+i(u)$ changes it by an element of the discarded image. This induces $W\otimes_AE\to T$, inverse to the map induced by $q\otimes1_E$. Thus the kernel of $q\otimes1_E$ is exactly the image of $i\otimes1_E$. Consequently a module is flat exactly when tensoring with it also preserves injections.

## ↑ Ancestors (7)

1. [Tensor product of modules](tensor-product-of-modules.md)
2. [Module theory](module-theory-split.md)
3. [Commutative algebra](commutative-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-7/1/d/solution.md)
