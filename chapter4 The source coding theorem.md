### chapter4

> The source coding theorem

#### question1:how to measure the information content of a random variable?

​	in order to measure the information content of a random variable , we introduce to a notation -- <b>Ensemble</b>. According to the book, An ensemble X is a triple $ (X, A_x,P_x)$
where the outcome x is the value of a random variable. which takes on one of a set of possible values, $ A_x=\{a_1,...,a_i,...,a_I\} $ , having probabilities $ P_x=\{ p_1,...p_2,...,p_I\} $ ,with $ P(x=a_i)=p_i, p_i\geq0 and \sum {p(x=a_i)=1} $ 

1. with the help of Ensemble, we define <b>Shannon information content</b> :

$$
h(x=a_i) = log_2\frac{1}{p_i}
$$

it is a sensible measure of the information content of the outcome $ x=a_i $ .

2. here we define **entropy of the ensemble,** which is the same meaning of ensembles' average information content.
   $$
   H(X) = \sum_i{p_ilog_2\frac{1}{p_i}}
   $$

tips: the binary entropy function : $ H_2(p)=H(p,1-p)=plog_2\frac{1}{p}+(1-p)log_2\frac{1}{1-p} $

***

	#### question2: how to make an optimal strategy

​	With the definition above, here we have a think about how to make an optimal strategy (in the book it is illustrate by the Weighing Problem). The conclusion is that : the outcome of a random experiment is guaranteed to be most informative if the probability  distribution over outcomes is **uniform distribution**.

The submarine example and the game of 63.

***

#### Data compression

​	examples: ASCII characters

​	A simple data compression method: we simply count the number of the possible outcomes. If it is happened to be a power of 2,we thus define it as : **The raw bit content of X** $ H_0(X) = log_2{|A_x|} $ .

​	one of the most important property of the raw bit is that it is the **lower bound** for the number of binary questions that are always guaranteed to identify an outcome from ensemble X.