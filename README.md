# Introduction

&emsp;&emsp;丢番图方程的研究，可以追溯到古希腊或者更久远的时期。其研究的主要目的就是求解多项式方程的整数解或者有理数解(即在域 $$\mathbb{Z}$$ 或 $$\mathbb{Q}$$ 上的解).术语丢番图几何，是最近才起源，其源于丢番图方程在代数数论和代数几何上技巧的结合.一方面，寻找多项式方程的有理解的问题发挥了代数数论工具的力量，代数数论描述了多项式在环和域中解的位置。另一方面，一个多项式方程解的体系描述了一个代数簇，代数簇是一个几何对象。这两个观点之间的相互影响，相互作用便是丢番图几何的主题了.

&emsp;&emsp;最简单的丢番图方程也就是线性的方程

$$
aX+bY=c~~~~a,b,c \in \mathbb{Z}~~~~a~or~b \geq 0.
$$

&emsp;&emsp;这个方程总是有有理数解，其有整数解的充分必要条件是➡**当且仅当$$(a,b) = c$$**，如果能找到一个整数解，则可通过Euclid辗转相除法找出所有的解

&emsp;&emsp;下一个较难的方程为二次方程

$$
aX^2+bXY+cY^2+dX+eY+f=0~~~~a,...,f \in \mathbb{Z}~~~~a,b~or~c \geq 0.
$$


&emsp;&emsp;其描述的是圆锥截面，通过适当的线性变换（系数为有理数），上述二次方程可转变为下述的方程组

$$
AX^2+BY^2=C~~~~ellipse
$$ 
$$
~~~~AX^2-BY^2=C~~~~hyperbola
$$ 
$$
AX^2+BY^2=0~~~~parabola
$$ 

&emsp;&emsp;对于二次方程，下面👇给出了一个强有力的理论来解决它们

**$$Hasse-Minkowski~Theroem([Se~7,~\mathrm{IV}~Thm.~8])$$**

**&emsp;&emsp;令$$f(x,y) \in \mathbb{Q}[X,Y]$$是一个二次多项式.那么方程$$f(x,y)=0$$有有理数解$$(x,y)\in \mathbb{Q}^2 \Leftrightarrow $$ 存在$$(x,y) \in \mathbb{R}^2$$的解和$$(x,y)\in \mathbb{Q}^{2}_p~~\forall~prime~p.$$的解(这里$$\mathbb{Q}_p$$是$$p-adic$$数域)**

&emsp;&emsp;换言之，**二次多项式方程有$$\mathbb{Q}$$中的解$$\Leftrightarrow$$在每个$$\mathbb{Q}$$完全的域中有解**。现在我们通过Hasse的引理检验每一个$$\mathbb{Q}_p$$中的解，其实与在每一个有限域$$\mathbb{Z}/p\mathbb{Z}$$中的解是相同的.这样的话，在$$\mathbb{Z}/p\mathbb{Z}$$中通过二次互反律会变得更容易完成这检验.我们总结一下二次丢番图方程的分析步骤

* 在有限域分析方程[二次互反律]
* 使用这些信息在局部域$$\mathbb{Q}_p$$上研究方程[$$Hasse's~lemma$$] (也要研究$$\mathbb{R}$$上的)
* 把所有的局部信息凑在一起去观察整体域$$\mathbb{Q}$$[$$Hasse~principle$$]


&emsp;&emsp;那几何在哪儿呢？含两个变量的线性方程和二次方程定义了两类亏格为0的曲线簇.以上讨论表明我们有相当好的理解对于亏格为0的曲线上的算术理论，下一个非常简单的例子，亏格为1的曲线(含有两个变量的三次方程)上的算术性质，是本书主要的研究对象.这类曲线（椭圆曲线）的算术理论在最近的大部分研究中成为核心问题，并且椭圆曲线的算术理论在当下越来越复杂.更进一步，椭圆曲线的算术理论为更高亏格的曲线和更高维的(交换)代数簇上的猜想和技巧提供了一个标准的测试场地.

&emsp;&emsp;简要的概述一下这本书.在两章关于关于代数几何的基本知识的介绍之后，我们开始研究在代数闭域上的椭圆曲线的几何性质($$chapter~~\mathrm{III}$$).然后接着继续上述(前一章)的方案大纲同时探究椭圆曲线在有限域上的性质($$chapter\mathrm{V}$$);局部域上的性质($$chapter\mathrm{VI}~~\mathrm{VII}$$)和整体(数)域上的性质($$chapter\mathrm{VIII}~~\mathrm{IX}~~\mathrm{X}$$).在有限域和局部域上我们对椭圆曲线的理解是相当的满意的.然而，在次数大于2的多项式，类似的$$Hasse-Minkowski~Theroem$$结果是是错的.这意味着该定理对于次数为2的多项式从局部到全局的过渡会更加的弱.这个问题的研究会在$$chapter\mathrm{X}$$细述

&emsp;&emsp;椭圆曲线的理论是十分丰富，宽阔和非常令人惊讶的.这本书的原本目标是独立的提供关于椭圆曲线基本的算术性质的介绍，即使这样有限的目标也被表明野心太大了.上述描述的材料大约有一半是作者曾想包含进入书本内容中的。本书的读者将会发现对于遗漏的话题的一些简单的讨论和参考清单，相应的信息在附录$$C$$中.

&emsp;&emsp;我们的另一个独立的目标已经很成功了，当然，我们可以自由地陈述每个读者都应该知道的结论，即使这些证明远超出了这本书的范围.但是，我们已经很努力的不用这些结论去做进一步的删减，这样的做法有三个例外.第一个：我们没有证明在复数域$$\mathbb{C}$$上椭圆曲线在椭圆函数上是均匀的$$(\mathrm{VI}~5.1)$$,这个结论最适合在模函数方面讨论，模函数的话题已被我们遗漏。第二个：我们没有证明在局部域中，“非奇异”点在所有点的集合内是有限个的$$(\mathrm{VII}~6.2)$$.显然其可已被证明，通过十分明确的多项式计算$$(cf.~[Ta~6])$$，但是这个过程是冗长的,又因为空间不足而未被收录。最后一个：椭圆曲线上的整数点的研究，我们利用$$Roth$$的理论而不做出证明.但是关于证明的简单讨论在$$(\mathrm{IX}~8)$$给出，同时那些之后想了解更多样的细节的读者可以前往这里列出的参考资料。

&emsp;&emsp;阅读这本书的前提条件是非常适度的.我们假定读者们已具有初步的代数数论的理论知识.因此对数域，整数环，素理想，素理想分解，模(绝对值)，完备性等等是熟悉的.了解代数数论中任何基本的文本内容（比如$$La~2,Part~\mathrm{I}$$或者$$Bo-Sh$$）都应该是足够的了.假定熟悉复分析的基本原理，那么$$chapter\mathrm{VI}$$解决了在$$\mathbb{C}$$上的椭圆曲线问题,在$$chapter\mathrm{X}$$,我们将会需要一点群同调的知识，不过仅是$$H^0$$和$$H^1$$的，读者们会发现上同调事实上需要去读$$chapter~X$$给的附录$$B$$.最后，由于我们接近的主要是代数，这里会有些背景材料是代数几何方面的问题.在一方面，由于椭圆曲线的大量理论可以被发现用于显示方程和计算，我们不要求读者已经了解大量的代数几何知识.在另一方面,这是一本数论方面的而不是代数几何方面的书籍，没有理由去花费大半的书本内容从我们需要的代数数论知识的基本原理出发来展开，作为妥协，开始的前两章介绍了代数几何中的簇和曲线，陈述了我们需要的代数几何知识.给出了完备的知识参考，同时提供了足够多的证明以便读者能得到对于一些在代数几何中被使用的技巧的趣味.

&emsp;&emsp;大量的习题已被包含在每个章节的结尾，想要获得对该课题真正了解的读者，应尽可能多地尝试，部分习题在著作中有（特殊情况）结论。习题的注解和评论列表在本书的末尾.单星号的习题有时会很难，双星号的问题则是未解决的问题.

## Reference

&emsp;&emsp;参考书目使用方括号框起来的，例如$$[Ta~5,thm.6]$$.相互参考$$theorems,propositions,lemmas$$在相同的章节中通过圆括号给出，比如$$(4,3)$$,习题的参考是这样的$$(exer.~3.6)$$,从一个章节到另一个章节的参考或者附录前面是以罗马数字或字母开始，比如$$(\mathrm{IV}~3),(\mathrm{B}.2.1)$$