# 第3章 偏好

## 3.1 偏好

定义$X\subseteq \mathbb{R}^n$为消费者所有可选消费束的集合。

**偏好**：消费者对不同消费束按其喜好程度给出的排序关系。偏好关系定义在$X$上。

偏好是消费者对消费束的主观评价。消费者根据其偏好，在消费束中进行选择。

设$\textbf{x},\textbf{y} \in X$

**严格偏好**：$\textbf{x} \succ \textbf{y}$
表示消费者相较于$\textbf{y}$更喜欢$\textbf{x}$。

**无差异**：$\textbf{x}\sim\textbf{y}$
表示消费者认为$\textbf{x}$和$\textbf{y}$一样好。

**弱偏好**：$\textbf{x}\succeq\textbf{y}$
表示消费者认为$\textbf{x}$至少和$\textbf{y}$一样好（有偏好或无差异）。

## 3.2 理性选择公理

为了能够广泛运用“偏好”这一概念进行（数理化）分析，我们需要做出一些公理性的假设。以下四个假设称为**理性选择公理**。

**完备性**：假定任何两个消费束都可以比较。
完备性是说，只要有两个消费束，消费者就可以做出选择。这条假设排除了两个消费束无法比较的特殊情况。因而，若$\textbf{x}\succeq\textbf{y}$不成立，则一定有$\textbf{y}\succ\textbf{x}$。
因此，完备性说明，任何两个消费束都可以用$\succeq$来定义：
1. 严格偏好：$\neg(\textbf{y}\succeq\textbf{x})\Leftrightarrow\textbf{x}\succ\textbf{y}$
2. 无差异：$(\textbf{x}\succeq\textbf{y})\wedge(\textbf{y}\succeq\textbf{x})\Leftrightarrow\textbf{x}\sim\textbf{y}$
3. 弱偏好：$\textbf{x}\succeq\textbf{y}$

**反身性**：一个消费束至少和它自身一样好，即$\textbf{x}\succeq\textbf{x}$。
实际上，由反身性，显然可以得出：$(\textbf{x}\succeq\textbf{x})\wedge(\textbf{x}\preceq\textbf{x})\Leftrightarrow\textbf{x}\sim\textbf{x}$，即一个消费束一定和自身一样好。
反身性保证了消费者行为的一致性。

**传递性**：$(\textbf{x}\succeq\textbf{y})\wedge(\textbf{y}\succeq\textbf{z})\Leftrightarrow\textbf{x}\succeq\textbf{z}$
传递性排除了如“$\textbf{x}\succeq\textbf{y}$，$\textbf{y}\succeq\textbf{z}$，但却又有$\textbf{z}\succeq\textbf{x}$”这种矛盾的情况。在传递性假设下，消费者能够选出最佳消费束的*集合*。
传递性还说明，给定任意多个消费束，消费者都可以对它们进行排序。

**连续性**：对$\forall\textbf{y}\in X$, $\{\textbf{x}\mid \textbf{x}\succeq\textbf{y}\}$是开集。
连续性说明，若$\textbf{x}\succeq\textbf{y}$，则于$\textbf{x}$“相似”消费束也弱偏好于$\textbf{y}$，即对消费束的“微小”变动不会改变偏好关系。

## 3.3 无差异曲线

无差异曲线是一种描述偏好的方法。

设$\textbf{x}^* \in X$

**弱偏好集**：$\{\textbf{x}\mid \textbf{x}\succeq\textbf{x}^*\}$
**无差异曲线**：$\{\textbf{x}\mid \textbf{x}\sim\textbf{x}^*\}$

当只考虑两种商品时，弱偏好集和无差异曲线就可以在二维空间中画出来。

![](images/2022-04-04-21-16-06.png)

显然，无差异曲线是弱偏好集的下边界。

## 3.4 偏好的实例

下面给出几个常见、常用的偏好的例子（两种商品的情况）。

**完全替代**：消费者愿意按固定比例用一种商品替代另一种商品。

例如，消费者现在消费红铅笔（商品1）和蓝铅笔（商品2）。但其只关心铅笔的数量，而不关心铅笔的颜色。假设给定消费束为$(10,10)$，此时铅笔总数为$20$。显然，任何使得$x_1+x_2=20$的消费束$(x_1,x_2)$都无差异于$(10,10)$。
此时无差异曲线就是一系列斜率为$-1$的直线（替代比率就是1）。因为消费者只在意铅笔的数量，所以偏好的增加方向是右上方。

![](images/2022-04-04-21-24-58.png)

**完全互补**：消费者按固定比例消费两种商品。
例如，鞋子总是两只脚一起穿，也就是说左脚的鞋子（商品1）和右脚的鞋子（商品2）按$1:1$的固定比例消费。
给定消费束$(10，10)$，显然有$(x_1,10)\sim(10,10),x_1\ge 10$以及$(10,x_2)\sim(10,10),x_2\ge 10$。无差异曲线就是一系列$L$型的曲线，顶点就是那些左鞋数量等于右鞋数量的消费束。

![](images/2022-04-04-21-37-15.png)

**厌恶品（bads）**：消费者不喜欢的商品。
假设消费者喜欢香肠（商品1），不喜欢凤尾鱼（商品2），则凤尾鱼就是该消费者的厌恶品。
当消费者增加厌恶品的消费时，为了保持满意程度不变（在同一条无差异曲线上），就必须给其一定的嗜好品作为补偿（这是消费者主观上的要求），所以当厌恶品的消费增加时，嗜好品的消费也增加，此时无差异曲线是一系列斜率为正的直线。

![](images/2022-04-04-21-42-59.png)

偏好增加的方向是右下方（厌恶品消费量减少，嗜好品消费量增加）。

**中性商品**：消费者不在乎（无感）的商品。
假设消费者喜欢香肠，但对凤尾鱼无感。此时凤尾鱼就是该消费者的中性商品。
当两种商品中有一种是中性商品（设为商品2）时，偏好水平只取决于另一种普通商品（设为商品1），此时无差异曲线是一系列垂直线。偏好的增加方向是向右。

![](images/2022-04-04-21-46-59.png)

**餍足**：存在一个最佳的消费束，越靠近这个消费束偏好水平越高。
设消费者有餍足$(\overline{x}_1,\overline{x}_2)$，则无差异曲线如下图所示：

![](images/2022-04-04-21-53-27.png)

当消费者拥有两种商品都太少或者太多是，斜率为负。当两种商品中有一种太多时，斜率为正。这是因为当两种商品都太多时，这两种商品就都是厌恶品，同时减少这两种商品的消费会使得满意程度提高（反过来，当两种商品都太少时，应该同时增加两种商品的消费量）。当两种商品中的一种太多时，这种商品就成了厌恶品，减少对它的消费有利于满意程度的提高。

**离散商品**：只能按整数消费的商品。
假如商品1是离散商品，此时无差异曲线就是由一系列离散的点构成的点集。弱偏好集也不再是一个区域，而是一系列直线段。

![](images/2022-04-04-22-00-12.png)

## 3.5 良态偏好（well-behaved preferences）

为了便于分析，我们还需要对偏好做出一些假设。这些假设不仅简化了数学上的分析，并且在两种商品的情况下还能使无差异曲线具有良好的性态。例如，连续性假设排除了无差异曲线存在虚线部分的情况。

**单调性（MWG给出的定义）**：对$\forall\textbf{x},\textbf{y}\in X$，
若$\textbf{x} \gg \textbf{y}$，则$\textbf{x}\succ\textbf{y}$（弱单调性）
若$\textbf{x}\ge\textbf{y}$，且$\textbf{x}\neq\textbf{y}$，则$\textbf{x}\succ\textbf{y}$（强单调性）

注：
1. 符号“$\textbf{x} \gg \textbf{y}$”表示，对$\forall x_i,y_i\enspace(i=1,2,3,\cdots,n)$，都有$x_i>y_i$。因此，弱单调性要求$\textbf{x}$中每一种商品的消费量都要严格大于$\textbf{y}$中对应商品的消费量。
2. 强单调性只要求$\textbf{x}$中至少有一种商品的消费量大于$\textbf{y}$中对应商品的消费量，且$\textbf{x}$和$\textbf{y}$是不同的消费束。

单调性假设的意义在于：
第一，单调性排除了“无差异区域存在的可能”。

（补一张无差异区域的图）

第二，**单调性意味着无差异曲线的斜率是负数**，即无差异曲线从左上方向右下方倾斜。
解释一：任意给定一个消费束$(x_1,x_2)$，从这一点出发，如果向右上方移动（两种商品的消费量都增加），就会移动到一个更好的位置；如果向左下方移动（两种商品的消费量都减少），就会移动到一个更差的位置。因此，要想使得消费者的满意程度不变，就只能向左上方或右下方移动。

![](images/2022-04-04-23-28-38.png)

解释二：根据单调性假设的定义，如果当一种商品的消费量增加时另一种商品的消费量不变，那么消费者一定更喜欢新的消费束（强单调性）。所以，要想使得新的消费束和原来的消费束无差异，就必须在增加一种商品的消费量时减少另一种商品的消费量，这就意味着无差异曲线的斜率是负数。

第三，单调性使得效用函数（第4章）是单调增加函数。

**凸性**：对$\forall\textbf{x},\textbf{y},\textbf{z}\in X$，如果$\textbf{x}\succeq\textbf{z}$，$\textbf{y}\succeq\textbf{z}$，则对$\forall t \in [0,1]$，都有$t\textbf{x}+(1-t)\textbf{y}\succeq\textbf{z}$。

注：
1. $t\textbf{x}+(1-t)\textbf{y},t\in [0,1]$表示$\textbf{x}$和$\textbf{y}$的凸组合。
2. 这一定义等价于：对$\forall \textbf{z} \in X$，$\{\textbf{x}\mid\textbf{x}\succeq\textbf{z}\}$是凸集。因此凸性假设意味着弱偏好集是凸集。
3. 凸性强于单调性（单调性强于局部非饱和\餍足性）。

两种商品情况下的凸偏好如下图所示：

![](images/2022-04-04-23-21-15.png)

凸偏好的经济含义是：
1. “平均”消费束优于“极端”消费束。
2. 效用函数是拟凹函数。
   
我们还可以给出严格凸的定义：
**严格凸**：对$\forall t\in(0,1)$，以及$\forall\textbf{x},\textbf{y},\textbf{z}\in X, \textbf{x}\neq\textbf{y}$，若$\textbf{x}\succeq\textbf{z}$，$\textbf{y}\succeq\textbf{z}$，则有$t\textbf{x}+(1-t)\textbf{y}\succ\textbf{z}$

注：严格凸性使得效用函数是凹函数，且边际替代率递减。

当偏好满足完备性、反身性、传递性、连续性和单调性时（主要是传递性和单调性），就可以证明如下重要命题：
**同一个消费者的无差异曲线不会相交**
证明一：
当两条无差异曲线相交时，如下图所示：

![](images/2022-04-05-10-01-44.png)

由无差异曲线的定义，易知此时$\textbf{y}\sim\textbf{z}$，$\textbf{x}\sim\textbf{z}$。由偏好的传递性可知，$\textbf{x}\sim\textbf{y}$。
又因为$\textbf{x}\ge\textbf{y}$，且$\textbf{x}\neq\textbf{y}$，所以根据偏好的单调性，可得$\textbf{x}\succ\textbf{y}$，这与$\textbf{x}\sim\textbf{y}$矛盾！
综上所述，同一个消费者的无差异曲线不会相交。

证明二：
设$\textbf{y}\in X$，易知此时一定$\exist\textbf{x}\in X$，满足$\textbf{x}\ge\textbf{y}$且$\textbf{x}\neq\textbf{y}$。由偏好的（强）单调性可知，此时$\textbf{x}\succ\textbf{y}$。
记$A=\{\textbf{a}\mid\textbf{a}\succeq\textbf{y}\}$，$B=\{\textbf{b}\mid\textbf{b}\succeq\textbf{x}\}$。
假设$A\cap B\neq\empty$，则$\exist \textbf{c}\in A\cap B$。因此，$\textbf{y}\sim\textbf{c}$和$\textbf{x}\sim\textbf{c}$都成立。
又因为此时满足偏好的传递性，所以有$(\textbf{y}\sim\textbf{c})\wedge(\textbf{x}\sim\textbf{c})\Leftrightarrow\textbf{y}\sim\textbf{x}$，这显然与$\textbf{x}\succ\textbf{y}$矛盾！
综上，一定有$A\cap B=\empty$，即无差异曲线不相交。

良态偏好的几何意义：
**当消费者的偏好满足理性选择公理以及单调性和凸性时，无差异曲线就是一系列凸向原点的平行的连续曲线**。

## 3.6 边际替代率（重点）

**边际替代率（MRS）**：（保持偏好程度不变）消费者愿意用一种商品去替代（或交换）另一种商品的比率。

边际替代率的公式为：$MRS=\large\frac{\triangle x_2}{\triangle x_1}=\frac{dx_2}{dx_1}$

![](images/2022-04-05-10-21-07.png)

边际替代率代表了消费者对商品的**主观评价**。
例如，如果$MRS=\large\frac{\triangle x_2}{\triangle x_1}\normalsize=k$，则$\triangle x_2=k\cdot\triangle x_1$，意味着当消费者想增加$\triangle x_1$单位的商品1的消费时，其愿意放弃的商品2的数量是$|k|\cdot\triangle x_1$。令$\triangle x_1=1$，此时$\triangle x_2=k$，也就是说，在这一点上消费者认为一单位的商品1值$k$个单位的商品2。

当只考虑两种商品时，边际替代率就是无差异曲线的斜率。当消费者有良态偏好时，无差异曲线的斜率是负的，所以此时边际替代率一般是负数。

**预算线的斜率的经济含义（联系第2章）**：预算线的斜率$-\large\frac{p_1}{p_2}$表示*市场*愿意用一种商品去替代（或交换）另一种商品的比率。

显然，当$MRS\neq-\large\frac{p_1}{p_2}$时，消费者就有动机进行商品交换。

![](images/2022-04-05-10-37-00.png)

如图所示，图中的直线实际上就是预算线。在点$B$，预算线的斜率的绝对值大于无差异曲线的斜率的绝对值，即$\large\frac{p_1}{p_2}\normalsize>\vert MRS\vert$，由此可得$\large\frac{p_1}{p_2}\normalsize\cdot\triangle x_1>\vert MRS\vert \cdot\triangle x_1$。这意味着此时消费者实际用$\triangle x_1$换得的$\triangle x_2$（按市场交换率），大于其想用$\triangle x_1$换得的$\triangle x_2$（按主观交换率）。因此在该点，消费者就有动机用商品1交换商品2.
而在点$C$则相反（$\large\frac{p_1}{p_2}\normalsize<\vert MRS\vert$），消费者此时有动机用商品2交换商品1。
这种交换会一直进行下去，直到$\large\frac{p_1}{p_2}\normalsize=\vert MRS\vert$，在图中表示为点$A$。