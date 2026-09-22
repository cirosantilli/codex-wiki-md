<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce a checked exception class, for example in its own source file:
```
public final class ItDoesDependOn extends Exception {
    private final MLType.TypeVar variable;
    public ItDoesDependOn(MLType.TypeVar variable) {
        this.variable = variable;
    }
    public MLType.TypeVar getVariable() { return variable; }
}
```
Declare the required abstract method in `MLType`:
```
public abstract void mustNotDependOn(TypeVar a)
    throws ItDoesDependOn;
```
Within the nested `TypeVar` class implement it by an identity check:
```
public void mustNotDependOn(TypeVar a) throws ItDoesDependOn {
    if (this == a) throw new ItDoesDependOn(a);
}
```
Within the nested `Arrow` class implement it recursively:
```
public void mustNotDependOn(TypeVar a) throws ItDoesDependOn {
    from.mustNotDependOn(a);
    to.mustNotDependOn(a);
}
```
The parameter denotes an actual non-null [type variable](../../../../../../type-variable.md) returned by the factory; checking object identity distinguishes different variables without confusing their printed names. [Structural induction](../../../../../../structural-induction.md) on the [abstract syntax tree](../../../../../../abstract-syntax-tree.md) proves the [occurs check](../../../../../../occurs-check.md): a variable node contains the queried variable exactly when the identities match, and an arrow contains it exactly when either component does. The first detected occurrence throws and propagates the checked exception; normal return proves absence. Both subclass methods must declare the exception, and callers must catch or declare it.

For $(\alpha\to\beta)\to(\beta\to\gamma)$, either recursive branch detects each of $\alpha,\beta,\gamma$, whereas a distinct $\delta$ is absent and the call returns. **A recursive identity-based occurs check throws exactly when the queried variable occurs.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
