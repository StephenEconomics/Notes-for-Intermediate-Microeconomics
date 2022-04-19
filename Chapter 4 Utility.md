# 第4章 效用

## 4.1 从偏好到效用

**效用是一种描述偏好关系的方法**。我们为每一个消费束指派一个“效用”，用效用间的大小关系来描述这些消费束之间的偏好关系。由此我们引出效用函数的概念。

**效用函数**是为每个可能可能的消费束指派一个数字（即效用）的方法，它指派给受较多偏好的消费束的数字大于指派给受较少偏好的消费束的数字。也就是说，若$\textbf{x}\succeq\textbf{y}$，则$u(\textbf{x})\ge u(\textbf{y})$。

例子：现在有$A,B,C$三个消费束，且$A\succ B\succ C$，那么我们应该如何为这三个消费束指派效用以表示上述偏好关系呢？这里给出三种方法。

![](images/2022-04-12-21-07-21.png)

可以发现，只要我们指派的效用能够正确表示消费束的偏好关系，那么这样的效用指派方式就是合理的。因此，**效用函数不唯一**，只要能找到一种为消费束指派效用的方法，我们就能找到无限多种指派效用的方法。而实现种“从一到无限”的方法就是正单调变换。

**正单调变换**：若函数$f:\mathbb{R} \rightarrow \mathbb{R}$是严格单调增函数，即$f^\prime(\cdot)>0$，则称$f$是一个正单调变换。若用$u$表示原本的效用函数，则$f(u)$就是经过正单调变换后的新的效用函数。

可以证明，**正单调变换不改变效用函数对偏好的描述**（即指派的效用对消费束的排序是一样的）。

证明：

根据效用函数的定义，可知$\textbf{x}\succeq\textbf{y}\Leftrightarrow u(\textbf{x})\ge u(\textbf{y})$。
又由正单调变换的定义，可知$f[u(\textbf{x})]\ge f[u(\textbf{y})] \Leftrightarrow u(\textbf{x})\ge u(\textbf{y})$。
因此可以得到，$\textbf{x}\succeq\textbf{y} \Leftrightarrow f[u(\textbf{x})]\ge f[u(\textbf{y})] $。

注：对于一些比较难处理效用函数形式（如根号、幂次等），可以对其进行正单调变换以转换成容易处理的函数形式。

## 4.2 基数效用和叙述效用

当我们用效用来描述偏好关系时，一个自然而然的问题就是：效用的绝对数值是否有意义？根据对这个问题的不同回答可以划分出两种不同的效用思想：基数效用和序数效用。

**基数效用理论**：效用的绝对数值有意义，反映了消费者的满意程度，可以加总。
注：“可以加总”这一点可以用如下例子来理解。一杯牛奶给消费者带来的效用是$10$，一勺蜂蜜给消费者带来的效用是$5$，则基数效用理论认为一杯牛奶加一勺蜂蜜给消费者带来的效用是$15$。

**序数效用理论**：效用的绝对数值没有意义，只表示对消费束的排序，不能加总。

实际上，基数效用理论存在一系列的问题：
1. 基数效用过于主观、不普适。根据基数效用理论，当$u(\textbf{x})=2u(\textbf{y})$时，消费者对$\textbf{x}$的喜爱程度是对$\textbf{y}$的喜爱程度的两倍。但是问题在于我们如何说明“两倍的喜爱程度”。可能会存在这样一种情况：消费者$A$认为多花两倍的钱代表两倍的喜爱程度，消费者$B$认为多等两倍的时间代表两倍的喜爱程度。也就是说，我们很难找到一个适用于所有人的度量具体的喜爱程度的方式。
2. 效用的可加性不一定成立。一杯牛奶给消费者带来的效用是$10$，一勺蜂蜜给消费者带来的效用是$5$，但是一杯牛奶加一勺蜂蜜给消费者带来的效用很有可能不是$15$（如果消费者很喜欢牛奶加蜂蜜的组合，那么效用就会大于$15$；如果消费者很不喜欢牛奶加蜂蜜的组合，那么效用就会小于$15$）。

并且，为了确定是哪一个消费束被消费者选择，我们只需要知道哪一个消费束更受偏好。因此，知道哪一个消费束的效用更大就足以让我们对消费者的选择行为进行分析。知道效用具体有多大并不会对我们分析选择行为有额外的帮助。

综上，选择用序数效用进行分析的原因是：
1. 基数效用过于主观和模糊，且不普适。
2. 效用的可加性不一定成立。
3. 序数效用足以描述消费者的选择行为。

## 4.3 效用函数

效用函数一定存在吗？答案是否定的。

例如，当偏好不满足传递性时，可能会有$A\succ B\succ C \succ A$，但是显然不存在一个函数$u$使得$u(A)>u(B)>u(C)>u(A)$，因为这违背了实数系的基本公理。

因此，效用函数要存在，就必然要满足一定条件。

**效用函数存在定理（Debreu, 1964）**：定义$X\subseteq \mathbb{R}^n_+$是所有可选消费束的集合。如果$X$上的偏好$\succeq$满足完备性、自反性、传递性和连续性，则存在一个效用函数$u:X\rightarrow \mathbb{R}$，使得$\textbf{x}\succeq\textbf{y} \Leftrightarrow u(\textbf{x})\ge u(\textbf{y})$。

效用函数存在定理的简单证明（假设单调性成立）：

一、代数方法：

设$\textbf{e}=(1,1,\cdots,1) \in X$为一个消费束。
易知对$\forall \textbf{x}= (x_1,x_2,\cdots,x_n)\in X$，都存在实数$a$满足$a>0$且$a\ge\max\{x_1,x_2,\cdots,x_n\}$，并使得$a\cdot \textbf{e}\ge \textbf{x}\ge 0\cdot \textbf{e}$。
当偏好满足单调性时，则有$a\cdot\textbf{e}\succeq\textbf{x}\succeq 0\cdot\textbf{e}$。
同时，因为偏好满足连续性，所以存在$a(\textbf{x})\in[0,a]$，使得$a(\textbf{x})\cdot\textbf{e}\sim\textbf{x}$。此时，$a(\cdot)$就是一个效用函数！

![](images/2022-04-13-15-58-29.png)

e.g. $\textbf{x}\succeq\textbf{y} \xrightleftharpoons \\a(\textbf{x})\cdot\textbf{e}\succeq a(\textbf{y})\cdot\textbf{e} \xrightleftharpoons{Monotonicity} a(\textbf{x})\ge a(\textbf{y})$

二、几何方法（Varian, 2014, Chapter 4）：

从几何上来说，效用函数就是一种为无差异曲线标记数字使得受较多偏好的无差异曲线得到较大数字的一种方法。

在只考虑两种商品的情况下，可以在$x_1x_2$空间中画出曲线$x_2=x_1$，沿着这条曲线测度每条无差异曲线离原点的距离，并按距离的大小顺序标记每条无差异曲线。

![](images/2022-04-12-22-08-05.png)

当偏好满足完备性、自反性、传递性、连续性和单调性时，曲线$x_2=x_1$和每条无差异曲线只会相交一次，并且无差异曲线越靠近右上方，其被标记的数字就越大，因此上述标记无差异曲线的方法就是一个效用函数。

## 4.4 边际效用（基数效用论）

**边际效用（Marginal Utility, MU）**：（保持其他商品的消费量不变）当商品$i\enspace(i=1,2,3,\cdots,n)$的消费量有微小变动时，效用的变化率。

$MU_i=\lim\limits_{\triangle x_i\to 0}\Large\frac{u(x_i+\triangle x_i,\textbf{x}_{-i})}{\triangle x_i}\normalsize=\Large\frac{\partial u(\textbf{x})}{\partial x_i}$

注：$\textbf{x}_{-i}=(x_1,x_2,\cdots,x_{i-1},x_{i+1},\cdots,x_n)$

根据边际效用的定义，$\triangle U=MU_i\cdot\triangle x_i$表示商品$i$的消费量变动$\triangle x_i$导致的效用的变动。特别地，令$\triangle x_i=1$，则$\triangle U=MU_i$，因此$MU_i$可以表示1单位商品$i$带来的边际效用。

注：
1. 边际效用隐含了效用的绝对数值是有意义的这一观点。因此边际效用中所说的“效用”指的是基数效用。
2. 描述同一偏好的不同效用函数求出的边际效用很可能不同。
3. **边际效用递减（假设）**：$\Large\frac{\partial MU_i}{\partial x_i}\normalsize=u_{ii}(\textbf{x})<0$

补充：货币的边际效用和基数效用论的消费者均衡思想

假若只考虑两种商品，商品1的价格为$p_1$，商品2的价格为$p_2$，且$p_1$和$p_2$由市场决定。则1单位货币可以购买的商品1和商品2的数量分别是$\Large\frac{1}{p_1}$和$\Large\frac{1}{p_2}$。因此，当1单位货币用于购买商品1时，带来的效用增量为$\triangle U_1=MU_1\cdot(\Large\frac{1}{p_1})\normalsize=\Large\frac{MU_1}{p_1}$。同理，当1单位货币用于购买商品2时，带来的效用增量为$\triangle U_2=\Large\frac{MU_2}{p_2}$。对于一个理性的消费者而言，如果$\Large\frac{MU_1}{p_1}\normalsize>\Large\frac{MU_2}{p_2}$，那么该消费者就会选择把这1单位货币用于购买商品1。反之则用于购买商品2。

由于边际效用递减，显然，在消费者购买商品的过程中，会逐渐达到这样一个均衡：$\Large\frac{MU_1}{p_1}\normalsize=\Large\frac{MU_2}{p_2}\normalsize=\lambda$，其中$\lambda$表示货币的边际效用。

## 4.5 效用函数的例子

### 4.5.1从效用函数到无差异曲线

我们可以用效用函数来定义无差异曲线：$\{\textbf{x}\mid u(\textbf{x})=k\}$。因此，在知道效用函数的情况下，如果想画出一条无差异曲线，只需要标出所有使得$u(\textbf{x})=k$的点$\textbf{x}$就可以了。

例如，已知$u(x_1,x_2)=x_1x_2$。令$x_1x_2=k$，解得$x_2=\Large \frac{k}{x_1}$，则无差异曲线如下图所示$(k=1,2,3,\cdots)$。

![](images/2022-04-13-11-29-45.png)

注意，**正单调变换不改变无差异曲线的形状**。因为已经证明正单调变换不改变效用函数对偏好的描述，所以正单调变换后无差异曲线的形状自然不变。在上述的例子中，对$u$进行正单调变换得到$v(x_1,x_2)=u^2=x_1^2x_2^2$，则根据$v$画出的无差异曲线和上图是一致的。

### 4.5.2 常用的效用函数（两种商品的情况）

这里给出几个常见的效用函数的例子。

**完全替代**：$u(x_1,x_2)=ax_1+bx_2$，其中$a$和$b$是用来测度商品1和商品2对消费者的“价值”的两个正数。
如果用基数效用来理解，则$a=MU_1$，$b=MU_2$

例：若消费者认为，要使其放弃一单位商品1，就必须给其2单位的商品2作为补偿，则该消费者的效用函数为？

显然，该消费者的偏好是完全替代的。并且，对该消费者来说，1单位的商品1值2单位的商品2，所以$MU_1=2MU_2=2b$，不妨设$b=1$，则$MU_1=2$，$MU_2=1$。所以该消费者的效用函数为$u(x_1,x_2)=2x_1+x_2$。

**完全互补**：$u(x_1,x_2)=\min\{ax_1,bx_2\}$，其中$a$和$b$是用来描述固定的消费比例的正数。
当满足$ax_1=bx_2$时，两种商品会被完全成比例地搭配消费（没有商品被浪费），此时商品1和商品2有固定的消费比例：$\Large\frac{x_2}{x_1}\normalsize=\Large\frac{a}{b}$。

以第3章中所举的左脚鞋子和右脚鞋子的完全互补偏好为例，消费者只关心最终有多少双鞋，因此我们自然选择用鞋子的双数来描述其偏好（即用鞋子的双数来指派效用）。而鞋子最终能有多少双取决于右脚鞋子数量$x_1$和左脚鞋子数量$x_2$中较小的那一个。所以该消费者的效用函数为$u(x_1,x_2)=\min\{x_1,x_2\}$。

这很容易验证，已知$(10,10)\sim(x_1,10)\sim(10,x_2)$，其中$x_1,x_2\ge10$。此时显然有$u(10,10)=u(x_1,10)=u(10,x_2)=10$。

例：某消费者喜欢1杯茶加2匙糖，则该消费者的效用函数为？

显然，该消费者的偏好是完全互补的。当消费者消费$x_1$杯茶时，要使得没有茶或者糖被浪费，则必须有$x_2=2x_1$匙糖。因此对该消费者而言，茶和糖有固定的消费比例：$\Large\frac{x_2}{x_1}\normalsize=\Large\frac{2x_1}{x_1}\normalsize=2=\Large\frac{a}{b}$。不妨令$a=1$，则$b=\Large\frac{1}{2}$。效用函数表示为$u(x_1,x_2)=\min\{x_1,\Large\frac{1}{2}\normalsize x_2\}$。

**拟线性效用**：$u(x_1,x_2)=v(x_1)+x_2$。若考虑边际效用递减，则还需假设$v''(x_1)<0$。

拟线性效用的所有无差异曲线都可以理解为由曲线$-v(x_1)$上下垂直平移得到的（令$u(x_1,x_2)=k$，解得$x_2=-v(x_1)+k$）。

![](images/2022-04-13-16-18-36.png)

注：
1. 拟线性效用主要用于理论分析，可以简化计算。
2. 对拟线性效用函数而言，$MU_1=v'(x_1)$，$MU_2=1$。因此商品1和商品2的边际效用无关。

**Cobb-Douglas效用函数**：$u(x_1,x_2)=x_1^c+x_2^d$，其中$c,d>0$。

根据Cobb-Douglas效用函数绘制的无差异曲线如下图所示：

![](images/2022-04-13-16-23-47.png)

可以看出：1. Cobb-Douglas偏好是典型的良态偏好（无差异曲线凸向原点）。2. $c$和$d$取值的不同会使无差异曲线的图像有所不同。

在求解有关Cobb-Douglas效用函数的效用最大化问题时，下面这两种正单调变换可以有效地简化计算：

一、取自然对数

$v(x_1,x_2)=\ln{u}=c\ln{x_1}+d\ln{x_2}$

二、幂变换

设$v(x_1,x_2)=x_1^cx_2^d$，$u(v)=v^{\large\frac{1}{c+d}}$。

因为$u'(v)=\Large\frac{1}{c+d}\normalsize\cdot v^{\large\frac{1-c-d}{c+d}}>0$，所以$u(\cdot)$是一个正单调变换，效用函数可以被写为$u(x_1,x_2)=x_1^{\large\frac{c}{c+d}}x_2^{\large\frac{d}{c+d}}$。

记$a=\Large\frac{c}{c+d}$，则$\Large\frac{d}{c+d}\normalsize=1-\Large\frac{c}{c+d}\normalsize=1-a$，于是有：$u(x_1,x_2)=x_1^a+x_2^{1-a}$。

因此，我们总是可以对Cobb-Douglas效用函数进行正单调变换，使其指数和为1。

## 4.6 边际替代率和边际效用

容易证明，边际替代率和边际效用在*数学上*有一定的代数关系。

回忆边际替代率（MRS）的含义。
**边际替代率（第3章）**：（保持偏好程度不变）消费者愿意用一种商品去替代（或交换）另一种商品的比率。

方法一：全微分

在引入效用工具后，“保持偏好程度不变”就意味着保持效用不变。

若效用函数可微，为分析如何使两种商品的消费量发生“微小”变动以使得效用不变，我们可以对效用函数求全微分，并令其等于0。

$du=\Large\frac{\partial u}{\partial x_1}\normalsize dx_1+\Large\frac{\partial u}{\partial x_2}\normalsize dx_2=MU_1\cdot dx_1+MU_2\cdot dx_2=0$

可以解得：$MRS_{12}=\Large\frac{dx_2}{dx_1}\normalsize=-\Large\frac{\Large\frac{\partial u}{\partial x_1}}{\Large\frac{\partial u}{\partial x_2}}\normalsize=-\Large\frac{MU_1}{MU_2}$

方法二：隐函数求导法

保持效用不变用效用函数可以表示为：方程$u(x_1,x_2)=u_0$始终成立。

若效用函数可微，对方程$u(x_1,x_2)=u_0$两边同时对$x_1$求导，可得：

$\Large\frac{\partial u}{\partial x_1}\normalsize + \Large\frac{\partial u}{\partial x_2}\frac{dx_2}{dx_1}\normalsize=0$

可以解得：$MRS_{12}=\Large\frac{dx_2}{dx_1}\normalsize=-\Large\frac{\Large\frac{\partial u}{\partial x_1}}{\Large\frac{\partial u}{\partial x_2}}\normalsize=-\Large\frac{MU_1}{MU_2}$

综上，当效用函数可微时，有：

$MRS_{12}=\Large\frac{dx_2}{dx_1}\normalsize=-\Large\frac{MU_1}{MU_2}$

还可以证明：**用描述同一偏好的不同效用函数求出的MRS是一样的**。

直观解释：因为正单调变换不改变无差异曲线的形状，所以自然正单调变换不会改变无差异曲线的斜率。因此，用描述同一偏好的不同效用函数求出的MRS是一样的。

数理方法证明：对效用函数$u(x_1,x_2)$，取严格单调增函数$f:\mathbb{R}\rightarrow\mathbb{R}$作正单调变换$f[u(x_1,x_2)]$，则：

$MRS_{12}=-\Large\frac{\Large\frac{\partial f(u)}{\partial x_1}}{\Large\frac{\partial f(u)}{\partial x_2}}\normalsize=-\Large\frac{f'(u)\cdot (\Large\frac{\partial u}{\partial x_1}\normalsize)}{f'(u)\cdot (\Large\frac{\partial u}{\partial x_2}\normalsize)}\normalsize=-\frac{\Large\frac{\partial u}{\partial x_1}}{\Large\frac{\partial u}{\partial x_2}}=-\Large\frac{MU_1}{MU_2}$

补充：边际替代率递减

**边际替代率递减**：$-\Large\frac{\partial |MRS_{ij}|}{\partial x_i}\normalsize<0$，即在保持效用水平不变的情况下，随着商品$i$消费的增加，消费者愿意放弃的商品$j$的数量会减少。

注意：**边际效用递减与边际替代率递减无关，二者不能互推！**
