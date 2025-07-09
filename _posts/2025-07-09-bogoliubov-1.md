---
title:  "从一个真空到另一个真空：Bogoliubov变换"
mathjax: true
layout: post
categories: media
---

最近接触到了一个奇怪的问题：对于标量场$$X$$，在平直时空里面，$$3X\to X$$的过程是不能发生的。原因很简单，由于动量守恒，不妨选择$$ \vec{p}_{X_1}+\vec{p}_{X_2}+\vec{p}_{X_3}=\vec{p}_{X_{\rm put}}=\vec{0} $$，那么，就有$$E_{\rm in}=3m_X>E_{\rm out}=m_X$$。然而，考虑标量场与环境之间存在能量或者动量交换的情况，这样3到1的反应就可以发生了。对于另一种情况，$$3X\to X'$$，其中$$X'$$是$$X$$的激发态，那么标量势的非线性效应也能产生3到1的转换。具体来说，考虑下面的有效场论

$$V(\Phi)=\frac{1}{2}m_X^2\Phi^2 - \frac{\lambda}{4}\Phi^4 $$


考虑$$\Phi $$的波函数由下面两部分叠加

$$ \Phi(t, \mathbf{r}) = \Phi_g(t, \mathbf{r})+\Phi_r(t, \mathbf{r})$$

其中下标$$g, r$$分别表示基态和自由态波函数。显然，势能中的$$\Phi^4$$项展开之后得到

$$\Phi^4=(\Phi_g+\Phi_r)^4 = \Phi_g^4 + 4\Phi_g^3\Phi_r +\cdots $$

这样就引入了一个$$3X_g\to X_r$$的反应。其他的$$2\to 2, 1\to 3$$以及$$0\to 4 $$反应不是被相空间压低，就是被禁戒。这个简单的玩具模型可以用来大量消耗某种凝聚的基态粒子——例如超辐射云。下面从EFT和相变（PT）的角度，讨论另一个玩具模型：


# 1. 背景：时间依赖的Hamltonian
对于具有Higgs势的标量场，我们很熟悉其由单圈修正给出的有限温度形式：$$V(\phi)=V_0(\phi)+V_1(\phi) $$，其中单圈修正同时包含零温与有限温度修正$$ V_1=V_1^0+V_1^T$$。我们用一个时间依赖的形式描述标量场EFT，例如暴涨理论，如下

$$V(\phi)=-\frac{1}{2}\mu^2\phi^2+\lambda(t)\phi^4 $$

考虑标量场包含两部分：一个随时间演化的“均值”部分，以及同时与位置、时间有关的“涨落”部分，即

$$\phi(t,\mathbf{r})\equiv \phi_0(t)+\delta\phi(t,\mathbf{r}) $$

得到与$$\delta \phi$$相关的作用量部分

$$ S[\delta \phi] =\int d^4x \left[\frac{1}{2} \partial_\mu \delta \phi \partial^\mu \delta \phi -  \frac{1}{2} m_{\text{eff}}^2\left(t \right)\delta \phi ^2 +\mathcal{O}(\delta \Phi ^4 )\right]$$

其中的有效质量由势能二阶导数给出，即

$$m_{\rm eff}^2(t) =\mu^2-12\lambda(t)\phi_0^2(t) $$

可见，当$$ \lambda(t)$$足够大，使得$$ m_{\rm eff}^2=0$$时，相变发生。这个标量场满足的运动学方程为

$$\left(\Box+m_{\rm eff}^2(t)\right)\delta\phi(t,\mathbf{x})=0 $$

# 2. 相变前后的波函数
不妨将发生相变的时间定为$$ t=0$$，波函数可以在相变以前(in)和以后(out)两组基下面展开

$$\delta\phi(t,\mathbf{x})=\int\frac{d^3k}{(2\pi)^3}\left[a_k^{\rm in}u_{k}^{\rm in}(t)\mathrm{e}^{\mathrm{i}k\cdot x}+\mathrm{h.c.}\right]=\int\frac{d^3k}{(2\pi)^3}\left[a_k^{\rm out}u_{k}^{\rm out}(t)\mathrm{e}^{\mathrm{i}k\cdot x}+\mathrm{h.c.}\right] $$

每一组基都满足对易关系 $$[a_k, a_{k'}^{\dagger}]=(2\pi)^3\delta^3(k-k') $$。注意到这两组基定义了两个不同的真空

$$a_k^{\rm in}\left|0_{\rm in}\right>=0, \; a_k^{\rm out}\left|0_{\rm out}\right>=0 $$

相变只是势能（或者势能的一阶导）不连续，波函数本身是连续并且光滑的，这样就可以把相变前后的波函数接起来:

$$ t<0: \; u_k^{\rm in}(t)=\frac{1}{\sqrt{2\omega_{k,i}}}\mathrm{e}^{-\mathrm{i}\omega_{k,i}t}$$

$$ t>0: \;, u_k^{\rm in}(t)=A_k\mathrm{e}^{-\mathrm{i}\omega_{k,f}t}+B_k\mathrm{e}^{\mathrm{i}\omega_{k,f}t}$$ 




