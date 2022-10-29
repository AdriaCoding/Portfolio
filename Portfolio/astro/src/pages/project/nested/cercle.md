**Problema 3.** *Considerem l'aplicació
$T_\lambda : S^1 \rightarrow S^1$, definida per
$T_\lambda(\theta) = \theta + \lambda \:(mod1)$. Estem identificant
$S^1 \equiv \mathbb{T} \cong \mathbb{R}/\mathbb{Z}$. També podriem
pensar en l'aplicació $T_\lambda$ com
$T_\lambda(e^{2 \pi \theta i}) = e^{2 \pi (\theta + \lambda) i}$.
Demostreu que les òrbites de $T_\lambda$ són denses en $S^1$ si i només
si $\lambda$ és irracional.*\
\
\
Comencem per observar que si
$\lambda \in \mathbb{N} \Rightarrow O_{T_\lambda}(\theta) = {\theta}$.\
Sigui $\lambda \in \mathbb{Q}$ i $\frac{p}{q}$ la seva fracció
irreductible , l'enèssim element de l'òrbita és
$T_\lambda^n(\theta) = \theta + \frac{p}{q} \ n \: (mod 1)$. En
particular, $T_\lambda^q(\theta) = \theta + p \: (mod 1) = \theta$ i
l'òrbita és periòdica amb $O_{T_\lambda}(\theta) = q$.\
Per tant, com que estem considerant que $\lambda \in \mathbb{R}$, una
òrbita $O_{T_\lambda}(\theta)$ només pot ser densa si
$\lambda \in \mathbb{R} \setminus \mathbb{Q}$.\
\
Per poder demostrar la implicació cap a l'esquerra cal primer definir
una distància a $S^1$. L'aplicació $d(x,y) = (x-y) \: (mod 1)$, verifica
$\forall x,y,z \in S^1$ el següent:

-   $d(x,y) \geq 0$ amb igualtat$\iff x-y \in \mathbb{Z} \iff x = y$ a
    $S^1$

-   $d(y,x) = -(x-y) \: (mod 1) = (x-y) \: (mod 1) = d(x,y)$

-   $d(x,z) = (x-y+y-z)\: (mod 1) = ((x-y) \: (mod 1) + (y-z) \: (mod 1)) \: (mod 1) = d(x,y) + d(y,z) \: (mod 1) \leq d(x,y) + d(y,z)$

I per tant, $d$ és una distància a $S^1$.\
\
Partim ara de que $\lambda$ és un irracional fix i suposem que
$\exists I \subset S^1$ obert tal que
$O_{T_\lambda}(\theta) \cap I = \varnothing \quad \forall \theta \in S^1$
amb $I = (a,b)$ i $d(a,b) = \epsilon$.\
Suposem que $\exists n, m$ tals que: $$\begin{aligned}
d := d(T_\lambda^n(\theta), T_\lambda^m(\theta)) = (\theta + \lambda m - \theta - \lambda n) \: (mod 1) = (m-n)\lambda \: (mod 1) < \epsilon\end{aligned}$$
$$\begin{aligned}
     \Rightarrow d(\theta,T_\lambda^{n-m}(\theta)) = (\theta - \theta -(n-m)\lambda) \: (mod 1) = d \end{aligned}$$
Si comencem des del punt $\theta$ i anem aplicant $T_\lambda^{n-m}$, ens
desplaçarem per $S^1$ fent petites passes de mida d i eventualment
caurem dins de I.\
Per tant, s'ha de tenir que
$\forall m,n \: d(T_\lambda^n(\theta), T_\lambda^m(\theta)) \geq \epsilon \Rightarrow |O_{T_\lambda}(\theta)| \leq \frac{1}{\epsilon}$,
contradicció amb el fet de que $\lambda$ és irracional.

$\blacksquare$
