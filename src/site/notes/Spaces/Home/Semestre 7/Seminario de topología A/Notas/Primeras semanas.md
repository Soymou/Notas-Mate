---
{"dg-publish":true,"permalink":"/spaces/home/semestre-7/seminario-de-topologia-a/notas/primeras-semanas/"}
---

# Definiciones básicas y construcciones


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/haz-vectorial/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




>[!definition] Haz vectorial
 >Un **haz vectorial $n$-dimensional** es un mapa (continuo) $p: E \to B$ junto con una estructura de espacio vectorial en $p^{-1}(b)$ para cada $b \in B$, de la tal manera que la siguiente condición de trivialización se cumple: Hay un cubierta abierta de $B$ por conjuntos abiertos $U_{\alpha}$ para cada uno de los cuales existe un homeomorfismo $h_{\alpha}: p^{-1}(U_{\alpha}) \to U_{\alpha}\times \mathbb{R}^{n}$ que manda a $p^{-1}(b)$ a $\{ b \}\times \mathbb{R}^{n}$ por un isomorfismo de espacios vectoriales para cada $b \in U_{\alpha}$.
 >El espacio $B$ es llamado espacio base, el espacio $E$ es el espacio total y los espacios vectoriales $p^{-1}(b)$ son las fibras.

</div></div>


> [!example]
> El producto o haz trivial $E= B \times \mathbb{R}^{n}$ con $p$ la proyección en el primer factor.

> [!example]
> Si hacemos que $E$ sea el espacio cociente de $I \times \mathbb{R}$ bajo las identificaciones $(0,t)\sim (1,-t)$, entonces la proyección $I \times \mathbb{R} \to I$ induce un mapa $p: E \to \mathbb{S}^{1}$ que es un 1-haz vectorial. Como $E$ es homeomorfo a la banda de Möbius con su círculo frontera removido, llamamos a este haz vectorial el haz de Möbius.

 > [!example]
> El haz tangente a la esfera unitara $\mathbb{S}^{n}$ en $\mathbb{R}^{n+1}$, un haz vectorial $p: E \to \mathbb{S}^{n}$ donde $E=\{ (x,v) \in \mathbb{S}^{n}\times \mathbb{R}^{n+1}|~ x \perp v \}$ y pensamosa $v$ como un vector tangente a $\mathbb{S}^{n}$ trasladadndolo de tal manera que su cola esté en $x$. El mapa $p: E \to \mathbb{S}^{n}$ manda a $(x,v)$ a $x$. Para construir trivializaciones locales, escogemos un punto $x \in \mathbb{S}^{n}$ y sea $U_{x} \subseteq \mathbb{S}^{n}$ el hemisferio abierto que contiene a $x$ y está acotado por el hiperplano por el origen ortogonal a $x$. Definimos $h_{x}: p^{-1}(U_{x}) \to U_{x} \times p^{-1}(x) \cong U_{x} \times \mathbb{R}^{n}$ por      $h_{x}(y,v)=(y,\pi_{x}(v))$, donde $\pi_{x}$ es la proyección ortogonal en el hiperplano $p^{-1}(x)$. 
> Entonces $h_{x}$ es una trivialización local pues $\pi_{x}$ se restringe a un isomorfismo de $p^{-1}(y)$ a $p^{-1}(x)$ para cada $y \in U_{x}$.
> 

> [!example]
> El haz normal a $\mathbb{S}^{n}$ en $\mathbb{R}^{n+1}$, un haz de líneas $p: E \to \mathbb{S}^{n}$ donde $E$ consiste de los pares $(x,v) \in \mathbb{S}^{n}\times \mathbb{R}^{n+1}$ tales que $v$ es perpendicular al plano tangente a $\mathbb{S}^{n}$ en $x$, en otras palabras, $v=tx$ para alguna $t \in \mathbb{R}$. El mapa $p: E \to \mathbb{S}^{n}$ está dado por $p(x,v)=x$. Para construir trivializaciones locales, podemos hacer la proyección ortogonal sobre la fibra $p^{-1}(x)$.
> 

> [!example]
> El $n$-espacio proyectivo real $\mathbb{R}P^{n}$ es el epacio de lineas en $\mathbb{R}^{n+1}$ por el origen. Como cada línea intersecta a la esfera unitaria $\mathbb{S}^{n}$ en un par de puntos antípodas, podemos pensar a $\mathbb{R}P^{n}$ como el espacio cociente de $\mathbb{S}^{n}$ en donde los puntos antípodas han sido identificados. El *haz de líneas canónico* $p: E \to \mathbb{R}P^{n}$ tiene como espacio total al subespacio de $\mathbb{R}P^{n}\times \mathbb{R}^{n+1}$ que consiste de los puntos $(l,v)$ con $v \in l$, y $p(l,v)=l$. De nuevo, las trivializaciones locales se pueden construir con la proyección ortogonal en las fibras $p^{-1}(x)$.
> Hay también un espacio proyectivo infinito dimensional $\mathbb{R}P^{\infty}$ que es la unión de todos los espacios proyectivos finito dimensionales $\mathbb{R}P^{n}$ bajo las contenciones $\mathbb{R}P^{n}\subseteq \mathbb{R}P^{n+1}$ que vienen de las inclusiones naturales $\mathbb{R}^{n+1}\subseteq \mathbb{R}^{n+2}$. La topología que usamos en $\mathbb{R}P^{\infty}$ es la topología débil, donde un conjunto es abierto en $\mathbb{R}P^{\infty}$ si y sólo si intersecta a cada $\mathbb{R}P^{n}$ en un conjunto abierto. Las inclusiones $\mathbb{R}P^{n}\subseteq \mathbb{R}P^{n+1}$ inducen inclusiones correspondientes entre los haces canónicos, y la unión de todos ellos es el haz canónico sobre $\mathbb{R}P^{\infty}$.

> [!example]
> El haz canónico de líneas sobre $\mathbb{R}P^{n}$ tiene un complemento ortogonal, el espacio $E^{\perp}= \{ (l,v) \in \mathbb{R}P^{n}\times \mathbb{R}^{n+1}| v \perp l \}$. La proyección $p: E^{\perp} \to \mathbb{R}P^{n}$, $p(l,v)=l$, es un haz vectorial con fibras los subespacios ortogonales $l^{\perp}$ de dimensión $n$. Las trivializaciones locales se pueden construir de nuevo con la proyección ortogonal.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/isomorfismo-de-haces-vectoriales/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




> [!definition] Isomorfismo de haces 
> Un isomorfismo entre haces vectoriales $p_{1}: E_{1} \to B$ y $p_{2}: E_{2} \to B$ sobre el mismo espacio base $B$ es un homeomorfismo $h:E_{1} \to E_{2}$ que manda cada fibra $p_{1}^{-1}(b)$ en la fibra correspondiente $p_{2}^{-1}(b)$ mediante un isomorfismo entre espacios vectoriales. Usamos la notación $E_{1} \cong E_{2}$ para denotar que $E_{1}$ y $E_{2}$ son isomorfos.

</div></div>

> [!example]
> El haz normal de $\mathbb{S}^{n}$ en $\mathbb{R}^{n+1}$ es isomorfo al espacio producto $\mathbb{S}^{n} \times \mathbb{R}$ por el mapa $(x,tx) \mapsto (x,t)$.

> [!example]
> El haz tangente a $\mathbb{S}^{1}$ es también isomorfo al haz trivial $\mathbb{S}^{1}\times \mathbb{R}$, via $(e^{i\theta},ite^{i\theta}) \mapsto (e^{i\theta},t)$ para $e^{i\theta} \in \mathbb{S}^{1}$ y $t \in \mathbb{R}$.

> [!example]
> El haz de Möbius es isomorfo al haz canónico de líneas sobre $\mathbb{R}P^{1} \cong \mathbb{S}^{1}$. $\mathbb{R}P^{1}$ es barrido por una linea que está rotando un angulo de $\pi$, así que los vectores en estas líneas barren un rectángulo $[0,\pi]\times \mathbb{R}$ con los dos extremos $\{ 0 \}\times \mathbb{R}$ y $\{ \pi \}\times \mathbb{R}$ identificados. La identificacion es $(0,x) \sim (\pi,-x)$ pues rotar un vector un ángulo de $\pi$ produce su negativo.

# Secciones

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/seccion-de-un-haz-vectorial/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




> [!definition] Sección de un haz
> Una **sección** de un haz vectorial $p:E \to B$ es un mapa $s: B \to E$ que asigna a cada $b \in B$ un vector $s(b)$ en la fibra $p^{-1}(b)$. La condición $s(b) \in p^{-1}(b)$ también se puede escribir como $p \circ s = Id_{B}$.

</div></div>


Todo haz vectorial tiene una sección canónica, la sección cero, cuyos valores en cada fibra es el vector $0$. Frecuentemente identificamos la sección cero con su imagen, un subespacio de $E$ que se proyecta homeomorficamente dentro de $B$ por $p.$ 
A veces uno puede distinguir haces no isomorfos mirando los complementos de sus secciones 0, pues cualquier isomorfimos entre haces vectoriales $h: E_{1} \to E_{2}$ debe llevar la sección cero de $E_{1}$ a la sección cero de $E_{2}$, así que los complementos de las secciones en $E_{1}$ y $E_{2}$ deben ser homeomorfos. Por ejemplo, podemos ver que el haz de Möbius no es isomorfo al haz producto $\mathbb{S}^{1}\times \mathbb{R}$, pues es complemento de la sección cero es conexo para el haz de Möbius y disconexo para el haz producto.
En el otro extremo estaría una sección cuyos valores nunca son cero
