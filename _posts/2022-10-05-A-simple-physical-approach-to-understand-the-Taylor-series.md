---
layout: post
title: A simple physical approach to understand the Taylor series
tags: Maths Physics Intro
description: Do you know that the displacement formula with acceleration in one dimension which you had learned in Physics class actually reveals the existence of Taylor series implicitly?
---

I still remember the first time that I meet the concept of **Taylor series** was in one AP calculus textbook. It's kind of a pity that the AP calculus textbook I was reading at that time didn't give any further explanation about why and how this formula came up, etc. So I just questioned myself about its formation and finally I did figured it out at that time by using the knowledge I've learned in Physics. I guess you may wonder why wouldn't I just search on the Internet and see the proof of **Taylor series**, in fact, I did do that, but didn't work for me at that point, since I lack too much Maths knowledge to understand that proof. Therefore I found a new way to help myself understand the **Taylor series** at that time.

Firstly, let us derive the displacement formula with acceleration in one dimension:

<div style="overflow: auto;">
$$
\begin{aligned}
\frac{\mathrm{d} x}{\mathrm{d} t} &=v_t \\
\\
\mathrm{d} x&=v_t \times \mathrm{d} t \\
\int_{t_0}^{t} \mathrm{d} x&= \int_{t_0}^{t}\left(v_t \right) \ \mathrm{d} t \\
x_t&=\int_{t_0}^{t}\left(v_t \right) \ \mathrm{d} t + x_0
\end{aligned}
$$
</div>

Similarly, we can use the same deriving method of:

<div style="overflow: auto;">
$$
\frac{\mathrm{d} x}{\mathrm{d} t} = v_t \quad \Rightarrow \quad x_t=\int_{t_0}^{t}\left(v_t \right) \ \mathrm{d} t + x_0
$$
</div>

To get:

<div style="overflow: auto;">
$$
\frac{\mathrm{d} v}{\mathrm{d} t} = a_t  \quad \Rightarrow \quad v_t=\int_{t_0}^{t}\left(a_t \right) \ \mathrm{d} t + v_0
$$
</div>

Then we substitute  $v_t$  into  $x_t$ , we would have:

<div style="overflow: auto;">
$$
x_t=\int_{t_0}^{t}\left(\int_{t_0}^{t}\left(a_t \right) \ \mathrm{d} t \right)\ \mathrm{d} t + v_0(t-t_0)    + x_0 \tag{1}
$$
</div>

Note that since $a_t$ is a constant (In fact, this is related to the **Principle of least action** in Physics: We assume that the accleration of any system must be a constant,
in other words: $\dfrac{\mathrm{d}^3 (x)}{(\mathrm{d} t)^3} = 0$ ), therefore we could get our displacement formula with acceleration:

<div style="overflow: auto;">
$$
x_t=\dfrac{a_t(t-t_0)^2}{2}+v_0(t-t_0)+x_0
$$
</div>

But the problem is: What if $a_t$ is not a constant anymore (And that situations do happen a lot in real life), for example, have you heard about presence of *jerk* ( $j_t =\dfrac{\mathrm{d} a}{\mathrm{d} t}$ ) before?

Then we need to deal with the equation  $(1)$  again, through using the same deriving method stated above, we could get:

<div style="overflow: auto;">
$$
\frac{\mathrm{d} a}{\mathrm{d} t} = j_t  \quad \Rightarrow \quad a_t=\int_{t_0}^{t}\left(j_t \right) \ \mathrm{d} t + a_0
$$
</div>

Next we substitute  $a_t$  into  $x_t$ , we can have:

<div style="overflow: auto;">
$$
x_t=\int_{t_0}^{t}\left(\int_{t_0}^{t}\left(\int_{t_0}^{t}\left( j_t\right) \ \mathrm{d} t  \right) \ \mathrm{d} t  \right)  \ \mathrm{d} t + \dfrac{a_0(t-t_0)^2}{2}+ v_0(t-t_0)+ x_0
$$
</div>

And using some derivatives form to substitute in that equation:

<div style="overflow: auto;">
$$
x_t=\int_{t_0}^{t}\left(\int_{t_0}^{t}\left(\int_{t_0}^{t}\left( j_t\right) \ \mathrm{d} t  \right) \ \mathrm{d} t  \right)  \ \mathrm{d} t + \dfrac{\ddot{x}_{t=t_0}(t-t_0)^2}{2!}+\dfrac{\dot{x}_{t=t_0}(t-t_0)}{1!}+ \dfrac{x_{t=t_0}}{0!}
$$
</div>

<div style="overflow: auto;">
$$
\text{Where } \dot{x}_{t} = \dfrac{\mathrm{d} x}{\mathrm{d} t}, \ddot{x}_{t} =\dfrac{\mathrm{d}^2 x}{(\mathrm{d} t)^2} \text{ and so on.}
$$
</div>

Now I believe that you could clearly see the presence of the **Taylor series** in this equation right?

Therefore if we keep iterating using the same method and let  $x_{t}=f(t)$ , we would be able to get the real **Taylor series** formula:

<div style="overflow: auto;">
$$
f(t)=\sum_{n=0}^{\infty }\left( \frac{f^{(n)}{'}({t=t_0})}{n!} \left(t-t_0\right)^{n}\right)
$$
</div>

This also indicate us the essence of **Taylor series**: Knowing all of its $n$th ($n$ is natural numbers) derivatives value at one point is equivalent to Knowing the primitive formula of a function.