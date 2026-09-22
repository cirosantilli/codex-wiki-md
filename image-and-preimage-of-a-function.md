# Image and preimage of a function

↑ **Parent:** [Set theory](set-theory-split.md)

The [image of a function](image-of-a-function.md) asks which outputs a chosen [set](set-split.md) of inputs reaches. A [preimage](preimage.md) asks which inputs reach a chosen [set](set-split.md) of outputs. Both constructions apply to every [function](function-split.md), including one that loses information by sending several inputs to the same output. Their difference is useful whenever a transformation must be followed forward or a condition on its result must be traced back.

Consider the [function](function-split.md) $f:A\to B$ with

$$
A=\{a,b,c,d\},\qquad B=\{0,1,2,3\},\qquad
f(a)=f(b)=0,\quad f(c)=1,\quad f(d)=2.
$$

Every input has exactly one output, but zero has two inputs and three has none. The full [image of a function](image-of-a-function.md) is $f(A)=\{0,1,2\}$, a proper [subset](subset.md) of the [codomain](codomain.md) $B$. Selecting inputs $\{a,c\}$ gives image $\{0,1\}$. Selecting outputs $\{0,2\}$ instead gives [preimage](preimage.md) $\{a,b,d\}$.

<a id="image-the-same-function-sends-a-selected-input-set-forward-and-pulls-a-selected-output-set-back"></a>
![](function-image-preimage-subset-flow.png)

**[Figure 5](#image-the-same-function-sends-a-selected-input-set-forward-and-pulls-a-selected-output-set-back). The same function sends a selected input set forward and pulls a selected output set back**. The full [codomain](codomain.md) contains three, which is never reached. Two inputs share output zero, so a [preimage](preimage.md) can recover a [set](set-split.md) of candidates without providing a unique [inverse function](inverse-function.md).

The [function](function-split.md) is not [injective](injective-function.md), because $f(a)=f(b)$, and is not [surjective](surjective-function.md) onto $B$, because three is absent from its image. Restricting only the [codomain](codomain.md) to $\{0,1,2\}$ makes the same rule [surjective](surjective-function.md); it remains noninjective. This separates the output set actually reached from the target set specified in the definition. The definitions of [images of a function](image-of-a-function.md) and [preimages](preimage.md), including the distinction from an [inverse function](inverse-function.md), are given in [Richard Hammack, Book of Proof, §12.6: Image and Preimage](https://richardhammack.github.io/BookOfProof/Main.pdf).

**Table of contents**

- [Image of a function](image-of-a-function.md)
- [Preimage](preimage.md)

## ↑ Ancestors (5)

1. [Set theory](set-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Fiber of a function](fiber-of-a-function.md)
- [Function collision](function-collision.md)
- [Image of a linear map](image-of-a-linear-map.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/4e/a/solution.md)
- [Surjective linear map](surjective-linear-map.md)
