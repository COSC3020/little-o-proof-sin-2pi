# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

## Answer 

We can let $f(n)\in o(g(n))$. Then , for all $c>0$, there exists an $n_0$ such that for all $n\ge n_0$, we have $f(n) < c g(n)$.

In particular, this means that for $c=1$, there exists an $n_0$ such that for all $n\ge n_0$, we have $f(n) < g(n)$.

So, there exists a positive constant ($c=1$) and there exists an $n_0$ such that for all $n\ge n_0$, we have $f(n) \le c g(n)$.

This is the definition of $f(n)\in O(g(n))$, so therefore $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$.
