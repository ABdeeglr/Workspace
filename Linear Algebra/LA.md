# 1第一线性代数

## 向量空间、向量和子空间

## 向量组、张成、张成空间、线性表示

## 线性无关

线性表示的唯一性-->线性无关-->哪种张成组最好

线性无关筛法

张成+线性无关-->基-->具有恰当长度的线性无关的张成组是基


\section{Vector and Vector Space}

如何建立起抽象的向量和向量空间的观念啊，笔者在此不多赘述，因为这是一种数学思想上的进步，难以用严格的形式逻辑来描述. 如果读者不认为下文中的定义是极其自然、是一种顺势而为而非人工雕琢的定义，那么请先读附录. 读者应当在对向量空间的定义感到非常自然时再进行进一步的理解.
\newline

\subsection{向量空间与子空间的定义}
\begin{definition}
    设$V$是一个非空集合，$K$是一个数域. $V$上有一个代数运算,称为加法,对任意$\alpha,\beta,\gamma\in V$满足



\begin{enumerate}
    \item $+(\alpha,\beta)\in V$;
    \item $+(\alpha,\beta)=+(\beta,\alpha)$
    \item $+(\alpha,+(\beta,\gamma))=+(+(\alpha,\beta),\gamma)$;
    \item $\exists \xi\in V$,满足$+(\alpha,\xi)=\alpha.$ $\xi$ 被称为零元素，记作 $0$;
    \item $\exists \lambda \in V$,满足$+(\alpha,\lambda)=0$,$\lambda$称为$\alpha$的加法逆元.
\end{enumerate}
$V$上有一个标量乘法运算，满足
\begin{enumerate}
    \item 对所有$k\in K，\alpha \in V$,$\times(k,\alpha)\in V;$
    \item 存在$q \in K$,使得$\times(q,\alpha)=\alpha$,$q$被称为标量乘法单位元，记作$1$;
\end{enumerate}
这两个运算具有分配性，即对所有的$k,l\in K$和$\alpha,\beta \in V$,满足

$$\begin{aligned}
    \times(a,+(\alpha,\beta))=+(\times(a,\alpha),\times(a,\beta))\\
    \times(a+b,\alpha)=+(\times(a,\alpha),\times(b,\alpha))\\
\end{aligned}$$
此时，称$V$在数域$K$上构成了线性空间,其中的元素被称为向量.\\
\end{definition} 

\newpage
\noindent 示例：
\begin{enumerate}
    \item $\mathbb{R}^4$在实数域上构成向量空间.
    \item 全体实值函数$f: \mathbf{R}\to \mathbf{R}$构成向量空间.\\
\end{enumerate}

\noindent 现在我们来引入子空间的概念. \\

\noindent 假设$V$是数域$K$上的线性空间，$\alpha$是$V$中的一个向量. 对于这个向量$\alpha$，它的线性组合是说形如$k\alpha,\quad k \in K$的向量. 类似的，对于多个向量构成的向量组$\alpha_1,\alpha_2,\cdots,\alpha_n$，它的线性组合是形如$k_1\alpha_1+k_2\alpha_2+\cdots+k_n\alpha_n$的向量. 把所有的线性组合放在同一个集合里，就得到了称为张成空间的概念.\\

\noindent 示例：假设$\alpha,\beta,\gamma$是向量空间$V$中任意三个向量，这三个向量的张成空间是其全体线性组合的集合，即$W=\{k\alpha+l\beta+m\gamma\}(k,l,m \in \mathbf{K})$. 在熟悉这一构造之后，我们简写成$W=span(\alpha,\beta,\gamma)$或者$\mathbf{L}(\alpha,\beta,\gamma)$. \\

\noindent 从过程角度，我们又说$\alpha,\beta,\gamma$张成了$W$,这和$W$是$\alpha,\beta,\gamma$的张成空间等价.\\

\noindent 容易验证的是，任意的张成空间$\mathbf{L}(\alpha_1,\alpha_2,\cdots,\alpha_n),(\alpha_1,\alpha_2,\cdots,\alpha_n\in V)$总是一个向量空间. 并且它还是$V$的一个子集. 基于这样的情况，我们提出了子空间的概念.\\

\begin{definition}
    设$W$是向量空间$V$的一个子集，如果$W$中的任意元素，对$V$中的加法和数乘运算构成向量空间，则称$W$是$V$的子向量空间，简称子空间.\\
\end{definition}
\newpage

\subsection{张成作为一种数学工具}

\noindent “张成”这一工具是强大的. 使用预先给定的（或者假设的）若干向量，来张成一个向量空间，本质上是一种朴素的构造法. 为了避免产生概念上的混乱，本小节将定义何为线性组合、线性表示和张成，读者需要注意的是，这只是为了在语言上获得便利，而非核心的概念.\\

\noindent 对于张成的讨论，最后会落到对向量组的研究上，这也是本小节的核心，即对向量组的线性相关性和秩的研究，这些概念是之后的重要概念的基础.\\

% 思路：同样的向量空间有不同的张成组，线性无关的张成组是好的. 如何从一个线性相关的向量组中找出无关组. 最终通过这一工具，我们得出了结论，一个有限维向量空间的张成组的长度不小于其线性无关的张成组的长度。这一认识

\begin{definition*}
    向量空间$V$中的一个向量组$v_1,v_2,\cdots,v_n$的\textbf{线性组合}是指形如
    $$
    a_1v_1+a_2v_2+\cdots+a_nv_n
    $$
    的向量，其中$a_1,a_2,\cdots,a_n$属于$V$对应的数域.
\end{definition*}

\begin{definition*}
    张成空间
\end{definition*}

\begin{definition*}
    张成
\end{definition*}

\noindent 张成的第一个显著作用，是区分了$\mathbb{R}^3$这样的向量空间和$R$上全体函数构成的向量空间之间的区别. 我们可以定义\textbf{有限维向量空间}是指那些能够被该空间自身中的有限个向量张成的空间，否则我们就说这个空间是\textbf{无限维}的. 在基础的线性代数中，我们只研究有限维的向量空间.\\

\noindent 接下来我们将解决一个问题，即怎样的张成是更好的. 考虑常见的$\mathbb{R}^3$空间，它可以有很多个张成组：
\begin{enumerate}
    \item $(1,0,0),(0,1,0),(0,0,1)$;
    \item $(1,0,0),(0,1,0),(0,0,1),(1,3,5)$;
    \item $(1,2,3),(2,2,3),(1,1,1)$.
\end{enumerate}
这三个张成组又都可以张成$\mathbb{R}^3$，\\

\newpage

\section{有限维向量空间的基}

\noindent 结合线性无关和张成组的概念,我们得到了基的定义. 基的优越性在于，其长度始终是不变的，或者说，选取不同的基，它的长度一定相同. 基于这样的发现，我们把基的长度称为向量空间的维数.并且，我们有一个和空间的维数公式
