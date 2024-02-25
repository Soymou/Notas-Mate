---
{"dg-publish":true,"permalink":"/semestre-7/geometria-algebraica/notas/categorias/"}
---


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/categoria/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Definición (Categoría)
Una categoría $\mathcal{C}$ consiste de:
1. Una clase $Obj(\mathcal{C})$ de objetos de la categoría.
2. Para cada par de objetos $A,B \in \mathcal{C}$, un conjunto $Hom_{C}(A,B)$ de morfismos con las siguientes propiedaes:
	- Para cada objeto $A \in \mathcal{C}$, existe al menos un morfismo $1_{A} \in Hom_{\mathcal{C}}(A,A)$, la identidad en $A$.
	- Se pueden componer morfismos: dos morfismos $f \in Hom(A,B)$ y $g \in Hom(B,C)$ determinan un morfismo $gf \in Hom(A,C)$. Es decir, para cada terna de objetos $A,B,C$ de $\mathcal{C}$ existe una función (de conjuntos) $Hom_{\mathcal{C}}(A,B) \times Hom_{\mathcal{C}}(B,C) \to Hom_{\mathcal{C}}(A,C)$ y la imagen del par $(f,g)$ es denotado por $gf$.
	- Esta regla de composición es asociativa: si $f \in Hom_{\mathcal{C}}(A,B)$, $g \in Hom_{\mathbb{C}}(B,C)$ y $h \in Hom_{\mathcal{C}}(C,D)$, entonces $(hg)f=h(gf).$
	- Los morfismos identidad son identidades con respecto a la composición: para todo $f \in Hom_{\mathcal{C}}(A,B)$ tenemos que $f 1_{A}=f=1_{B}f.$
	Una condición más es que los conjuntos $Hom_{\mathcal{C}}(A,B)$ y $Hom_{C}(C,D)$ sean disjuntos, a menos que $A=C$ y $B=D$. Es decir, si dos funciones son iguales, entonces sus fuentes y receptores son iguales.

</div></div>

Un morfismo de un objeto $A$ de una categoría $\mathcal{C}$ en sí mismo es llamado un *endomorfismo*, $Hom_{\mathcal{C}}(A,A)$ es denotado $End_{\mathcal{C}}(A)$. Es importante notar que la composición define una operación en $End(A)$.

## Ejemplo
La colección de todos los conjuntos junto con las funciones entre conjuntos forman una [[Conceptos/Categoría\|Categoría]]. Denotamos esta categoría por $Set$, de modo que $Obj(Set)=$ la clase de todos los conjuntos y para cada $A,B \in Obj(Set)$ $Hom_{Set}(A,B)= B^{A}$.

## Ejemplo
Supongamos que $S$ es un conjunto y $\sim$ es una relación en $S$ que es reflexiva y transitiva. Podemos codificar estos datos en una categoría:
- objetos: los elementos de $S$;
- morfismos: si $a$, $b$ son objetos, entonces sea $Hom(a,b)$ el conjunto que cosiste del elemento $(a,b) \in S \times S$ si $a\sim b$, y sea $Hom(a,b)=\emptyset$ en otro caso.
Tenemos que definir la composición de morfismos y verificar que se cumplen las condiciones de la definición de [[Conceptos/Categoría\|Categoría]]. Primero que nada, ¿tenemos identidades? Si $a$ es un objeto de $S$, tenemos que encontrar un elemento $$1_{a} \in Hom(a,a).$$
Esto es precisamente lo que estamos asumiendo al decir que $\sim$ es reflexiva: esto nos dice que para cada $a$, $a\sim a$; esto es, $Hom(a,a)$ consiste del único elemento $(a,a).$ Así que no tenemos elección y debemos tomar $$1_{a}=(a,a) \in Hom(a,a).$$ Para la composición, sean $a,b,c$ objetos y $$f \in Hom(a,b),~ g \in Hom(b,c);$$ tenemos que definir un morfimo correspondiente $gf \in Hom(a,c)$. Ahora $$f \in Hom(a,b)$$ esto nos dice que $Hom(a,b)$ es no vacío y, de acuerdo con la definción de morfismos en esta [[Conceptos/Categoría\|Categoría]] esto significa que $a\sim b$, y $f$ es de hecho el elemento $(a,b)$ de $S \times S$. Similarmente, $g \in Hom(b,c)$ esto nos dice que $b\sim c$ y $g=(b,c)$. Ahora $$a\sim b, ~ b\sim c \Rightarrow a\sim c$$
pues estamos asumiendo que $\sim$ es transitiva. Esto nos dice que $Hom(a,c)$ consiste del único elemento $(a,c)$. Entonces de nuevo no tenemos opción, debemos tomar $$gf=(a,c) \in Hom(A,C).$$ 
¿Esta operación es asociativa? Si $f \in Hom(a,b)$, $g \in Hom(b,c)$ y $h \in Hom(c,d)$, entonces necesariamente $$f=(a,b), g= (b,c), h=(c,d)$$ y $$gf=(a,c), hg=(b,d)$$
y, por lo tanto $$h(gf)=(a,d)=(hg)f$$
lo cual prueba la asociatividad. 
Es fácil ver que $1_{a}$ es una identidad respecto a esta composición.
La instancia más trivial de esta construcción se obtiene de un conjunto $S$ con la relación de equivalencia $=$; esto es, los únicos morfismos son los morfismos identidad. 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/categoria-discreta/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Definición 
Una [[Conceptos/Categoría\|categoría]] cuyos únicos morfismos son las identidades es llamada una categoría *discreta*.

</div></div>


Como otro ejemplo, consideremos la [[Conceptos/Categoría\|categoría]] que corresponde a equipar a $\mathbb{Z}$ con la relación $\leq$. Por ejemplo
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
2 \ar[r]\ar[dr] & 3 \ar[d,"1_3"] \ar[r] & 5 \ar[r] & 7\\
& 3\ar[rru] \ar[r] & 4 \ar[ru] &
\end{tikzcd}
\end{document}
```
Es un diagrama conmutativo elegido al azar del diagrama de esta [[Conceptos/Categoría\|categoría]]. 
Estas categorías son muy espaciales, cualquier diagrama que dibujemos en ellos es necesariamente conmutativo, y esto casi nunca es el caso.

## Ejemplo
Sea $S$ un conjunto. Definimos una categoría $\hat{S}$ haciendo:
- $Obj(\hat{S})= \mathcal{P}(S)$.
- Para $A, B$ objetos de $\hat{S}$ sea $Hom(A,B)$ el par $(A,B)$ si $A \subseteq B$ y sea $Hom(A,B)= \emptyset$ en otro caso.
La identidad $1_{A}$ consiste del par $(A,A)$ que es, de hecho, el único morfismo de $A$ en $A$. La composición se obtiene concatenando inclusiones: si hay morfismos $$A \to B, B \to C$$ en $\hat{S}$, entonces $A \subseteq B$ y $B \subseteq C$; así que $A \subseteq C$ y existe un morfismo $A \to C$. Checar que esta composición satisface los axiomas es un trabajo de rutina.

## Ejemplo 
Sea $\mathcal{C}$ una [[Conceptos/Categoría\|categoría]], y sea $A$ un objeto de $\mathcal{C}$. Vamos a definir una [[Conceptos/Categoría\|cateogría]] $\mathcal{C}_{A}$ cuyos elementos serán ciertos morfismos en $\mathcal{C}$ y cuyos morfismos serán ciertos diagramas en $\mathcal{C}$.
- $Obj(\mathcal{C}_{A})$ son todos los morfismos de un objeto de $\mathcal{C}$ en $A$; entonces, un objeto de $\mathcal{C}_{A}$ es un morfismo $f \in Hom_{\mathcal{C}}(Z,A)$ para algún objeto $Z$ de  $\mathcal{C}$. En dibujos, un objeto de $\mathcal{C}_{A}$ es una flecha $Z \xrightarrow{f} A$ en $\mathcal{C}$; estas se dibujan frecuentemente de arriba hacia abajo 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
Z \ar[d] \\
A
\end{tikzcd}
\end{document}
```
hola