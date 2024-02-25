---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/categoria/"}
---

# Definición (Categoría)
Una categoría $\mathcal{C}$ consiste de:
1. Una clase $Obj(\mathcal{C})$ de objetos de la categoría.
2. Para cada par de objetos $A,B \in \mathcal{C}$, un conjunto $Hom_{C}(A,B)$ de morfismos con las siguientes propiedaes:
	- Para cada objeto $A \in \mathcal{C}$, existe al menos un morfismo $1_{A} \in Hom_{\mathcal{C}}(A,A)$, la identidad en $A$.
	- Se pueden componer morfismos: dos morfismos $f \in Hom(A,B)$ y $g \in Hom(B,C)$ determinan un morfismo $gf \in Hom(A,C)$. Es decir, para cada terna de objetos $A,B,C$ de $\mathcal{C}$ existe una función (de conjuntos) $$Hom_{\mathcal{C}}(A,B) \times Hom_{\mathcal{C}}(B,C) \to Hom_{\mathcal{C}}(A,C)$$ y la imagen del par $(f,g)$ es denotado por $gf$.
	- Esta regla de composición es asociativa: si $f \in Hom_{\mathcal{C}}(A,B)$, $g \in Hom_{\mathbb{C}}(B,C)$ y $h \in Hom_{\mathcal{C}}(C,D)$, entonces $$(hg)f=h(gf).$$
	- Los morfismos identidad son identidades con respecto a la composición: para todo $f \in Hom_{\mathcal{C}}(A,B)$ tenemos que $$f 1_{A}=f=1_{B}f.$$
	Una condición más es que los conjuntos $Hom_{\mathcal{C}}(A,B)$ y $Hom_{C}(C,D)$ sean disjuntos, a menos que $A=C$ y $B=D$. Es decir, si dos funciones son iguales, entonces sus fuentes y receptores son iguales.