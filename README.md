# Module Theory

## Ring Modules
### Field
If the ring is actually a field (i.e., commutative and without any zero divisors), then the module is essentially a vector space over the field. For commutaive rings a right module is also a left module. Now, if $V$ is a vector space over a field $F$, then $V$ is also a module over the polynomial ring $F[x]$. We can assign a linear operator $T:V\rightarrow V$ and with respect to that define for $p(x)=a_nx^n+a_{n-1}x^{n-1}+\dots+a_0\in F[x]$,
$$p(x).v=a_nT^nv+a_{n-1}T^{n-1}v+\dots a_1Tv+a_0v$$
which is consistent with its restriction on $F$, where $v\mapsto a_0v$. Note that this extended action depends upon the linear operator $T$ chosen. If $T$ is identically $0$, we have the same module structure with no more information about the elements other than those of $F$. On the other hand, if $T$ is the shift operator, $\lb v_1,\dots,v_r\rb\mapsto \lb v_2,v_3,\dots, v_r, 0\rb$, we get a different $F[x]$-module structure of $V$.
