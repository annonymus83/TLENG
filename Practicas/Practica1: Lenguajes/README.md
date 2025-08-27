# Practica 1 : Lenguajes

### Ejercicio 1
Tenemos que $\Sigma = \{a, b\}$

* $\Sigma^0 = \{\lambda\}$
* $\Sigma^1 = \Sigma = \{a,b\}$
* $\Sigma^2 = \Sigma\Sigma = \{aa,ab,ba, bb\}$
* $\Sigma^* = \bigcup_{i \geq 0} \Sigma^i = \{\lambda, a, b, aa, ab, ba ,bb , aaa, aab, aba, abb, baa, bab, bba, bbb, ... \}$
* $\Sigma^+ = \bigcup_{i \geq 1} \Sigma^i =  \{ a, b, aa, ab, ba ,bb , aaa, aab,... \}$
* $|\Sigma| = 2$
* $|\Sigma^0| = 1$

### Ejercicio 2
Dado $\Sigma = \{ a, b \}$ vale:

* $\lambda \in \Sigma\ $, No vale. Es una palbra nula y por lo tanto no tiene simbolos.
* $\lambda \in \Sigma\ $ No vale, porque no pertence a $\Sigma$
* $\lambda \in \Sigma^+\ $ No, dado que la unión empieza desde $\Sigma^1$
* $\lambda \in \Sigma^*\ $ Si vale.
* $\Sigma^0 = \lambda\ $   No, es igual a un conjunto con $\lambda$ no a un elemento.
* $\Sigma^0 = \{\lambda\}\ $ Vale, por lo dicho arriba.

### Ejercicio 3
$\alpha = aab\ $ una cadena

* $\alpha^0 = \lambda$
* $\alpha^1 = \alpha.\lambda = \alpha = aab $
* $\alpha^2 = \alpha.\alpha = aabaab$
* $\alpha^3 = \alpha.\alpha.\alpha = aabaabaab$
* $\prod_{k = 0,...,3} \alpha^k = \alpha^0.\alpha^1.\alpha^2.\alpha^3 = \lambda.aab.aabaab.aabaabaab $
* $\alpha^r = baa$

### Ejercicio 4
Siendo $\alpha = abb$ y $\beta = acb$

* $\alpha.\beta = abb.acb = abbacb$
* $(\alpha.\beta)^r = bcabba$
* $\beta^r = bca$
* $\beta^r.\alpha^r = bcabba$
* $\lambda.\alpha = \alpha = aab$
* $\lambda.\beta = \beta = acb$
* $\alpha.\lambda.\beta = \alpha.\lambda.\beta = abbacb$
* $\alpha^2.\lambda^3.\beta^2 = aabaab.\lambda.acbacb = aabaabacbacb$

### Ejercicio 5
Tenemos un alfabeto $\Sigma$, $\ x,y \in \Sigma\ $ y $\ \alpha, \beta \in \Sigma^*$.

**a. $|𝑥.(𝑦.𝛼)| = 2 + |𝛼|$**

Por def. de longitud <br />
$|𝑥.(𝑦.𝛼)|= 1 + |(𝑦.𝛼)| = 1 + 1 + |𝛼| =    2 + |𝛼|$


**b. $|𝛼^𝑟| = |𝛼|$**

**Caso base**: $\alpha = \lambda \Rightarrow |\lambda^r| = |\lambda| = 0$


**Paso Inductivo:** <br />
HI : $|𝛼^𝑟| = |𝛼|$ <br />
Sea $\alpha = x.\alpha'$. Sup. que la HI vale para $\alpha'$:

```math
|\alpha^r| = |(x.\alpha')^r| \\ 
            =_{def. \bullet^r} |\alpha'^r.x| \\ 
            = 
```

**c. $|𝛼𝑥𝛽| = |𝑥𝛼𝛽|$**


**d. $|𝛼.𝛼| = 2|𝛼|$**


**e. $(𝛼.𝛽)^r = 𝛽^r.𝛼^r$**


**f. $(𝛼^r)^r = 𝛼$**


**g. $(𝛼^𝑟)^𝑛 = (𝛼^𝑛)^r$**