[TOC]

# Relations

## Relations

Let $S$ be a set. A **relation** on $S$ is a subset $R$ of $S\times S$.

 $R$ consists of ordered pairs $(s,t)$ with $s,t\in S$. For those ordered pairs $(s,t)\in R$, we write $s \sim t$ or $sRt$ and say $s$ is related to $t$.

> Example: Let $S=\mathbb{R}$ and define $a\sim b \iff a<b$. Here:
> $$
> R=\{(s,t)\in\mathbb{R}\times\mathbb{R}\ |\ s<t\}
> $$
>
> ---
>
> Example: Let $S=\mathbb{Z}$ and let $m$ be a positive integer. Define $a\sim b \iff a \equiv b\pmod{m}$, then:
> $$
> R=\{(s,t)\in\mathbb{Z}\times\mathbb{Z}\ |\ s \equiv t \pmod{m}\}
> $$
>

## Equivalence relations

Let $S$ be a set, and let $\sim$ be a relation on $S$. Then $\sim$ is an equivalence relation if the following three properties hold $\forall a,b,c\in S$:

- **Reflexivity**: $a\sim a$
- **Symmetry**: $a\sim b \implies b\sim a$
- **Transitivity**: $(a\sim b) \land (b\sim c) \implies a\sim c$

> Consider the two examples of relations in the previous section:
>
> - $R=\{(s,t)\in\mathbb{R}\times\mathbb{R}\ |\ s<t\}$
>   - **Reflexivity**: If $(x,x)\in R$, then for reflexivity we need $x<x$. However, this is clearly not the case, so this relation is **not reflexive**.
>   - **Symmetry**: If $(x,y)\in R$, then for symmetry we need $(x<y \implies y<x)$. Again, this is clearly not the case, so this relation is **not symmetric**.
>   - **Transitivity**: If $(x,y),(y,z)\in R$, then for transitivity we need $(x,z)\in R \iff x<z$. This is clearly the case, as $x<y<z \iff x<z$, so this relation **is transitive**.
>   - The relation is **not an equivalence relation** because not all three properties hold. 
> - $R=\{(s,t)\in\mathbb{Z}\times\mathbb{Z}\ |\ s \equiv t \pmod{m}\}$
>   - **Reflexivity**: If $(x,x)\in R$, then for reflexivity, we need $x\equiv x\pmod{m}$, which is clearly the case, so this relation **is reflexive**.
>   - **Symmetry**: If $(x,y)\in R$, then for symmetry, we need $x-y\equiv 0\pmod{m}\implies y-x\equiv 0\pmod{m}$. Note that $x-y=-(y-x)$, so this relation **is symmetric**.
>   - **Transitivity**: If $(x,y),(y,z)\in R$, then for transitivity we need $(x,z)\in R\iff x\equiv z \pmod{m}$. We have $x-y\equiv 0\pmod{m}$ and $y-z\equiv 0\pmod{m}$. Therefore, $(x-y)+(y-z)\equiv 0\pmod{m}$, giving us $x\equiv z\pmod{m}$, so this relation **is transitive**.
>   - The relation **is an equivalence relation** because all three properties hold.

## Equivalence classes

Let $S$ be a set and $\sim$ an equivalence relation on $S$. For $a\in S$, define
$$
cl(a)=\{s\ |\ s\in S,s\sim a\}
$$
Thus, $cl(a)$ is the set of things that are related to $a$. The subset $cl(a)$ of $S$ is called an equivalence class of $\sim$. The equivalence classes of $\sim$ are the subsets $cl(a)$ as $a$ ranges over the elements of $S$.

> Example: Consider the equivalence relation
> $$
> R=\{(s,t)\in\mathbb{Z}\times\mathbb{Z}\ |\ s \equiv t \pmod{m}\}
> $$
> Some various equivalence classes are:
>
> - $cl(0)=\{s\in\mathbb{Z} \ |\ s\equiv 0\pmod{m}\}$
>
> - $cl(1)=\{s\in\mathbb{Z} \ |\ s\equiv 1\pmod{m}\}$
>
>   $\quad\quad\quad\quad\quad\quad\quad\ldots$
>
> - $cl(m-1)=\{s\in\mathbb{Z} \ |\ s\equiv m-1\pmod{m}\}$
>
> We claim that these are all the equivalence classes. For if $n$ is any integer, then $\exists q,r\in \mathbb{Z} : n=qm+r$ with $0\leq r<m$. Then $n\equiv r\pmod{m}$, so $n\in cl(r)$, which is one of the classes listed above.

