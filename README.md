# Module Theory

## Ring Modules

### Group actions
Let $A$ be any set and $G$ a group written here in a multiplicative way. We define a *group action* as a function $G\times A\rightarrow A;~(g,a)\mapsto g.a\in A$ such that

(i) $g_1.\left( g_2.a\right)=\left( g_1g_2\right).a$ for all $g_1, g_2\in G$ and all $a\in A$;

(ii) $1_G.a=a$ for all $a\in A$.

We informally say that the group $G$ "acts on" the set $A$; $G\curvearrowright A$.

For some $g\in G$, define $\sigma_g:A\rightarrow A;~\sigma_g\left( A\right)=g.a$. Then, $\sigma_g\in S_A$, i.e., $\sigma_g$ is essentially a permutation of $A$. This is because, we can similarly have a $\sigma_{g^{-1}}$ that acts as both left and right inverse of $\sigma_g$, making $\sigma_g$ a bijective map. Indeed, $\left(\sigma_{g^{-1}}\circ\sigma_g\right)\left( a\right)=g^{-1}.\left( g.a\right)=\left( g^{-1} g\right).a=a$. Also, $\varphi:G\rightarrow S_A;~g\mapsto \sigma_g$ is a homomorphism, i.e., $\varphi\left( g_1g_2\right)\left( a\right)=\sigma_{g_1g_2}\left( a \right)=\left( g_1g_2\right).a=g_1.\left( g_2.a\right)=\sigma_{g_1}\left(\sigma_{g_2}\left( a\right)\right)=\varphi\left( g_1\right)\circ\varphi\left( g_2\right)\left( a \right)$.

### Annihilator
If we have an ideal $I$ of $R$ such that $rm=0$ for all $r\in I$ and $m\in M$, then $I$ is called an *annihilator* of $M$. In that case we can visualize $M$ as a ring module over the quotient ring $R/I$ where $(r+I).m:= rm$ where $r\in R,~m\in M$. In particular, if $I$ is maximal, then $R/I$ is a field and hence $M$ shall be a vector space.

Take for example a $\mathbb{Z}$-module $G$. This means that for some element $x$ in the module, $nx\in G$. Thus $G$ consists of distinct cycles of finite or infinite length and so is an abelian group. On the other hand, any abelian group is a $\mathbb{Z}$-module. Now, if there exists some $m\in\mathbb{N}$ such that $mx=0$ for all $m\in G$, then $m\mathbb{Z}$ is an annihilator of $G$. Even otherwise, simply $G$ is a $\mathbb{Z}/m\mathbb{Z}$-module. In particular for $m=p\in\mathbb{P}$ a prime, $\mathbb{Z}/m\mathbb{Z}$ has the structure of $\mathbb{F}_p$ and so $G$ is a vector space over $\mathbb{F}_p$.

We shall denote by $\text{Ann}_M(I)$ the annihilator of right ideal $I$ of $R$ in module $M$ as $$\text{Ann}_M(I):= \lbrace m\in M:am=0~\forall a\in I\rbrace$$. One can see that $\text{Ann}_M(I)$ is a submodule of $M$, because if $m_1, m_2\in\text{Ann}_M(I)$, then $m_1+\alpha m_2\in\text{Ann}_M(I)$ for all $\alpha\in R$.

On the other hand, for a submodule $N$ of $M$, the *annihilator* of $N$ in $R$ consists of those $r\in R$ for which $rn=0$ for all $n\in N$, denoted by $\text{Ann}_R(N)$. One can see that this is a two-sided ideal of $R$ as it absorbs any other element $r_1$ of $R$ this way: $r_1rn=r_10=0$, or $rr_1n=rn_1$ for some $n_1\in N$ and $rn_1=0$ for $r\in\text{Ann}_R(N)$.

### Field
If the ring is actually a field (i.e., commutative and without any zero divisors), then the module is essentially a vector space over the field. For commutaive rings a right module is also a left module. Now, if $V$ is a vector space over a field $F$, then $V$ is also a module over the polynomial ring $F[x]$. We can assign a linear operator $T:V\rightarrow V$ and with respect to that define for $p(x)=a_nx^n+a_{n-1}x^{n-1}+\dots+a_0\in F[x]$,

$$p(x).v=a_nT^nv+a_{n-1}T^{n-1}v+\dots a_1Tv+a_0v$$

which is consistent with its restriction on $F$, where $v\mapsto a_0v$. Note that this extended action depends upon the linear operator $T$ chosen. If $T$ is identically $0$, we have the same module structure with no more information about the elements other than those of $F$. On the other hand, if $T$ is the shift operator, $( v_1,\dots,v_r)\mapsto ( v_2,v_3,\dots, v_r, 0)$, we get a different $F[x]$-module structure of $V$.
