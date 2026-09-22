<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**No: a procedural parameter can carry an older lexical environment past a newer recursive activation.** Here is typed, Pascal-like pseudocode; a function-valued parameter is represented by a [programming closure](../../../../../closure-computer-programming.md), comprising code and its defining environment.

```
procedure dummy(): integer;
begin return 0 end;

procedure P(n: integer; f: procedure(): integer): integer;
    var x: integer;
    procedure Q(): integer;
    begin return x end;
begin
    x := n;
    if n = 1 then return P(2, Q)
             else return f()
end;

begin print P(1, dummy) end.
```

Call the first `P` activation $P_1$. It sets its own `x` to $1$ and passes the [programming closure](../../../../../closure-computer-programming.md) $(Q,P_1)$ into a recursive activation $P_2$. That activation sets its own `x` to $2$ and calls its parameter `f`. The resulting activation of `Q` has its [static link](../../../../../static-link.md) pointing to $P_1$, because that is where the passed procedure was defined. Its [dynamic link](../../../../../dynamic-link.md) points to $P_2$, because that is where it was called.

During this call the [dynamic chain](../../../../../dynamic-chain.md) contains `Q, P2, P1, main`, while `Q`'s [static chain](../../../../../static-chain.md) contains `Q, P1, main`. The newest surviving activation of `P` is $P_2$, but the [static chain](../../../../../static-chain.md) deliberately uses $P_1$. Correct [lexical scope](../../../../../lexical-scope.md) therefore prints $\boxed{1}$; blindly consulting `current[P]` would produce $2$. Both enclosing activations remain alive, so no issue of a returned procedure or dangling [pointer](../../../../../pointer-computer-programming.md) is involved.

The failed step in part (d) is precisely the assumption that the callee's lexical environment is a suffix of the direct caller's [static chain](../../../../../static-chain.md). A passed [programming closure](../../../../../closure-computer-programming.md) can specify a different, still surviving environment. An implementation supporting such calls must preserve that environment; a table implementation requires additional environment installation and restoration rather than merely consulting newest activations.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
