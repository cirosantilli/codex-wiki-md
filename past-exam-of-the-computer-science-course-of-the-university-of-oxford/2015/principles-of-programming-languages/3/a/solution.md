<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [programming closures](../../../../../closure-computer-programming.md) that receive evaluated arguments and return a computation in the chosen [computational monad](../../../../../computational-monad.md). A sufficient core of the semantic value domain is:

```
data Value = IntVal Integer
           | BoolVal Bool
           | Function ([Value] -> M Value)
```

Additional constructors may represent the other built-in values. Assume a [semantic environment](../../../../../semantic-environment.md) abstract data type with operations `lookupEnv :: Env -> Ident -> Value` and `extend :: Env -> [(Ident,Value)] -> Env`. The latter simultaneously adds the listed bindings, shadowing old bindings. Parameter names in one binding list are distinct, and calls have the expected arity.

Define [programming closure](../../../../../closure-computer-programming.md) construction separately; it does not run the body:

```
close :: Expr -> Env -> Value
close (Lambda xs body) rho =
  Function (\args -> eval body (extend rho (zip xs args)))

apply :: Value -> [Value] -> M Value
apply (Function f) args = f args
```

The four expression forms have the following semantic equations. Function position is evaluated first, followed by argument expressions from left to right:

```
eval :: Expr -> Env -> M Value

eval (Variable x) rho = result (lookupEnv rho x)

eval (Apply e es) rho =
  bind (eval e rho) (\f ->
    bind (evalArgs es rho) (\args -> apply f args))

eval e@(Lambda xs body) rho = result (close e rho)

eval (Let d body) rho =
  bind (defn d rho) (\rho' -> eval body rho')

evalArgs :: [Expr] -> Env -> M [Value]
evalArgs [] rho = result []
evalArgs (e:es) rho =
  bind (eval e rho) (\v ->
    bind (evalArgs es rho) (\vs -> result (v:vs)))
```

The two definition forms are:

```
defn :: Defn -> Env -> M Env

defn (Val x e) rho =
  bind (eval e rho) (\v -> result (extend rho [(x,v)]))

defn (Rec x e@(Lambda xs body)) rho = result rho'
  where
    rho' = extend rho [(x,v)]
    v = close e rho'
```

The ordinary definition evaluates its right-hand side in the old [semantic environment](../../../../../semantic-environment.md); its own name is not yet bound there. The recursive definition creates a [recursive closure](../../../../../recursive-closure.md) in the extended [semantic environment](../../../../../semantic-environment.md) containing itself. Because the right-hand side is a [lambda abstraction](../../../../../lambda-abstraction.md), constructing that [programming closure](../../../../../closure-computer-programming.md) does not evaluate its body. [Haskell](../../../../../haskell.md)'s [lazy evaluation](../../../../../lazy-evaluation.md) can tie this recursive data structure without requiring any extra fixed-point operation from the arbitrary [computational monad](../../../../../computational-monad.md).

[Lexical scope](../../../../../lexical-scope.md) is explicit: calling a [programming closure](../../../../../closure-computer-programming.md) extends the defining [semantic environment](../../../../../semantic-environment.md), and its parameters shadow bindings in that [semantic environment](../../../../../semantic-environment.md). The six requested constructs are therefore covered by

$$
\boxed{\operatorname{Variable},\ \operatorname{Apply},\ \operatorname{Lambda},\ \operatorname{Let},\ \operatorname{Val},\ \operatorname{Rec}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
