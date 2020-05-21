---
layout: post
author: rohan
tags: [arithmetic-geometry]
---
A genus 0 curve $$C$$ over $$K$$ is a twist of $$\mathbb{P}_K^1$$ i.e. a one-dimensional Bruaer-Severi variety. Such twists are classified by $$H^1(G_K, \text{Aut} (\mathbb{P}_K^1)) = H^1(G_K, \text{PGL}_1(\overline{K}))$$.

The exact sequence

$$ 1 \to \overline{K} \to \text{GL}_n \overline{K} \to \text{PGL}_n \overline{K} \to 1 $$.

gives rise to a map $$H^1(G_K, \text{PGL}_n\overline{K}) \to H^2(G_K, \overline{K}^\cross)$$. Hilbert's Theorem 90 says that $$H^1(G_K,  \overline{K}^\cross)$$ is trivial. Define the *Brauer group* $$\text{Br}(K)$$ to be $$H^2(G_K, \overline{K}^\cross)$$.  Thus in summary we have an injection


$$\{ \text{genus 0 curves} \ / \ K \} \into \Br(K)$$


Note that $$C(K) \neq \varnothing$$ if and only if $$C \isom \mathbb{P}_K^1$$. So $$C$$ has a rational point if and only if it is sent to the trivial class in the Brauer group.

Now recall the "fundamental exact sequence" coming from class field theory:


$$0 \to \text{Br}(\mathbb{Q}) \to \oplus_v \text{Br}(\mathbb{Q}_v) \to \mathbb{Q}/\mathbb{Z} \to 0$$

The direct sum in the middle of the exact sequence is taken over all places of $\Q$, including the infinite place.  

Putting these together, we have the following big diagram:



The top arrow is the expected arrow defined by base change from $$\mathbb{Q}$ to $$\mathbb{Q}_v$$. So, in particular, a genus 0 curve is trivial in $$\text{Br}(\mathbb{Q})$$ if and only if its base changes to all $$\mathbb{Q}_v$$ are all trivial in $$\text{Br}(\Q_v)$$. This implies the slogan ``a genus 0 curve over $$\mathbb{Q}$$ has a rational point if and only if it has a rational point over all completions $$\mathbb{Q}_p$$ and $$\mathbb{R}$$''; for quadratic forms, this is the Hasse-Minkowski theorem. In other words, genus 0 curves over $$\mathbb{Q}$$ satisfy the Hasse principle.
