---
layout: post
title: Why mathematicians choose "A linear subspace must have the additive identity" as one of the condition of the linear subspace but not "A linear subspace must be nonempty" ?
tags: Maths Intro
description: Actually they can do that, but why they don't? Because from the perspective of modern algebra...
---

When I first meet that condition (A linear subspace must have the additive identity) in the book of "Linear algebra done right", I felt it could be derived from "A linear subspace must be nonempty" + "A linear subspaces is closed under linear operations", which indicated that "A linear subspace must be nonempty" is a more fundamental condition than "A linear subspace must have the additive identity". So at that time, I believed that the replacement would definitely be correct, but I didn't really think through why mathematicians choose that not-most-fundamental one as a condition until I was introduced to modern algebra...

From the perspective of modern algebra, "A linear subspace must have the additive identity" is a more fundamental condition: Let me pull out a thing with the similar algebraic structure as an example -- submonoid, its conditions also include "A submonoid must have the binary-operation identity of the monoid it is contained in", but here we cannot replace this with "A submonoid must be nonempty":

Because let we construct a submonoid $(X,\*)$, where

<div style="overflow: auto;">
$$
X = \left \{  \begin{bmatrix} x  & 0\\\ 0 & 0 \end{bmatrix} \mid x \in \mathbb{R} \right \}  \subset  R^{2 \times 2} = \left\{  \begin{bmatrix} a  & b\\\ c & d \end{bmatrix} \mid a,b,c,d \in \mathbb{R}  \right \}
$$
</div>

And $\*$ is the matrix multiplication.

If we choose "A submonoid must be nonempty" not "A submonoid must have the binary-operation identity of the monoid it is contained in" as the condition, then $\begin{bmatrix} 1  & 0\\\ 0 & 0 \end{bmatrix}$ would be the matrix multiplicative identity of the submonoid $(X,\*)$, but this would conflict with the matrix multiplicative identity of the monoid $(R^{2 \times 2},\*)$ which it is contained in, which is the $\begin{bmatrix} 1  & 0\\\ 0 & 1 \end{bmatrix}$. Accordingly, "A submonoid must have the binary-operation identity of the monoid it is contained in" is proved to be a correct condition.

Now, let's get back to the topic of subspaces: Though the algebraic structure of the linear space allows the replacement of "A linear subspace must have the additive identity" with "A linear subspace must be nonempty" for the linear subspaces, considering other algebraic structures, it would be way more convenient if mathematicians use a generalized condition, and that's why I think they finally choose "A linear subspace must have the additive identity" for the linear subspace, but not "A linear subspace must be nonempty".