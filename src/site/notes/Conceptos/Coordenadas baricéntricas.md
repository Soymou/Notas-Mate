---
{"dg-publish":true,"permalink":"/conceptos/coordenadas-baricentricas/"}
---

# Definición
Supongamos que $\mathcal{K}$ es un complejo simplicial abstracto y $\left|\mathcal{K}\right|$ es su [[Conceptos/Realización geométrica de un complejo simplicial abstracto\|realización geométrica]]. Sea $\alpha \in \left|\mathcal{K}\right|$. En este caso, el valor de $\alpha(v)$ es la $v$-ésima coordenada de $\alpha$.
Definimos $t_{v}: \left|\mathcal{K}\right| \to [0,1]$ dada por $t_{v}(\alpha)=\alpha(v)$. Los elementos de la familia $$\{ t_{v} \}_{v \in \mathcal{V}}$$son llamados *coordenadas baricéntricas* de $\alpha$.
En este caso
$$\alpha=\sum_{v \in \mathcal{V}_{\mathcal{K}}} t_{v}(\alpha)\alpha_{v}= \sum_{v \in \mathcal{V}_{\mathcal{K}}}\alpha(v)\cdot \alpha_{v}.$$
Los valores $\{ t_{v}(\alpha) \}_{v \in \mathcal{V}_{\mathcal{K}}}$ son las coordenadas baricéntricas de $\alpha$.