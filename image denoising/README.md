Image-denoising with NLMS
===
Background
---
This a project in the digital signal process course, NLMS is a  Commonly used algorithm in signal processing. Although the effect of this algorith is not better than deep learning, it can be a exercise project to starter.

Install
-------
Download matlab from https://ww2.mathworks.cn/products/matlab.html, ensure that you have license of it.
  * toolbox you need: `Image Processing Toolbox`

Algorithm
-----
As you can see in the following figure, for a input x(n) with noise, LMS filter update error e(n)=y(n)-d(n) in every iterations to make e(n) smaller, and where y(n) is a signal after filtering and d(n) is a reference signal. A problem of this algorithm is how to choose d(n), which is our aim signal, if we know d(n) before filtering, we don't have to do filtering. So, when we use this algorithm in pratice, we can set d(n)=x(n) , don't be amazing. Also, this is the reason that LMS works but not very well, in another word, because we don't konw our aim signal, we just upate e(n) in each iteration, the outcome is output a signal y(n), which is close to d(n).
![image](https://github.com/WangSuhan/Image-denoising/blob/main/image%20denoising/LMS-picture.JPG)

Outcome
