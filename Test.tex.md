
# 1 Background

 승률과 손익비가 정해진 도박을 할 때, 원금의 얼만큼을 투자해야 파산하지 않으면서도 수익을 극대화할 수 있을까?

# 2 Definition
원금이 1,000,000원일 때, 원금의 절반을 투자하여 10% 수익이 났다면 잔고는 1,000,000 x (1 + 0.1 x 0.5) = 1,050,000원이 된다.

원금이 1,000,000원일 때, 원금의 절반을 투자하여 20% 손해가 났다면 잔고는 1,000,000 x (1 - 0.2 x 0.5) = 900,000원이 된다.

이를 일반화하면 다음과 같은 수식이 된다.

$$A_N=(1+fg)^W(1+fl)^L A_0$$
$W:\;number\;of\;wins$
$L:\;number\;of\;losses$
$N:\;number\;of\;trades\;(W+L=N)$
$p={W\over N}:\;probability\;of\;winning$
$q={L\over N}:\;probability\;of\;losing$
$A_N:\;account\;balance\;after\;N\;trades$
$A_0:\;initial\;account\;balance$
$g:\;\%gain\;(g>0)$
$l:\;\%loss\;(l<0)$
$f:\;optimal\;fraction$
$G:\;average\;growth\;rate$

$${A_N\over A_0}=(1+fg)^W (1+fl)^L$$
$$\log{A_N\over A_0}=W\log{⁡(1+fg)}+L\log⁡{(1+fl)}$$
$$\lim_{N\to∞}{1\over N}\log{A_N\over A_0}=\lim_{N\to∞}[{W\over N}⁡⁡\log⁡(1+fg)+{L\over N}\log⁡(1+fl)]$$
$$\lim_{N\to∞}{1\over N}\log{A_N\over A_0}=p\log⁡(1+fg)+q\log⁡(1+fl)$$
$$G=\lim_{N\to∞}{1\over N}\log{A_N\over A_0},maximize\;G$$
$$G=p\log⁡(1+fg)+q\log⁡(1+fl)$$
$$G'={gp\over 1+fg}+{lq\over1+fl}=0$$
$$gp(1+fl)+lq(1+fg)=0$$
$$gp+fglp+lq+fglq=0$$
$$(gp+lq)+fgl(p+q)=0$$
$$p+q=1$$
$$f=-{gp+lq\over gl}$$
$$\therefore f={p\over -l}-{q\over g}$$

# 3 Example
승률이 51%, 평균수익률 10%, 평균손실률 -10%인 매매전략의 최적비율은?
$f={0.51\over -(-0.1)}-{0.49\over 0.1}=0.2=20\%$



# 1 Background
승률과 손익비가 변하는 투자환경에서 원금의 얼만큼을 투자해야 파산하지 않으면서도 수익을 극대화할 수 있을까?

# 2 Definition
어떤 전략으로 주식을 매매했을 때 평균손익률을 m, 평균손익률의 편차를 s라고 하자.
매매를 통해 m+s의 수익을 얻을 수도, m-s의 손실을 입을 수도 있다.
원금의 일부만 투자하고, 나머지는 다른 계좌에 예금해 r만큼의 이자를 받는다고 가정한다.
X가 n회 매매한 결과라고 가정하면 m/n, s^2/n, r/n으로 바뀐다.
$X=\begin{cases}m+s&\text{if gain}\\m-s&\text{if loss} \end{cases}$
$E(X)=m,V(X)=s^2$
$A_n=A(1+(1-f)r+(m+s)f)^{1\over 2}(1+(1-f)r+(m-s)f)^{1\over 2}$
${A_n\over A}=(1+r+(m-r+s)f)^{1\over 2}(1+r+(m-r-s)f)^{1\over 2}$
$\ln⁡{A_n\over A}={1\over 2}\ln⁡(1+r+(m-r+s)f)+{1\over 2}\ln⁡(1+r+(m-r-s)f)$
$\ln⁡{A_n\over A}={1\over 2}\ln⁡(1+r+mf-rf+sf)(1+r+mf-rf-sf)$
$\ln⁡{A_n\over A}=\sum_{i=1}^n\{{1\over 2}\ln⁡(1+{r\over n}+({m\over n}-{r\over n}+{s\over \sqrt n})f)+{1\over 2}\ln⁡(1+{r\over n}+({m\over n}-{r\over n}-{s\over \sqrt n})f)\}$
$\ln⁡{A_n\over A}={n\over 2}\ln(⁡(1+{r\over n}+{m\over n}f-{r\over n}f)^2-{s^2\over n}f^2)$
$G=\ln⁡{A_n\over A}$


