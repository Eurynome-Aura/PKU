# Assignment #3: March月考

Updated 1537 GMT+8 March 6, 2024

2024 spring, Complied by 余汶青 生命科学学院



**说明：**

1）The complete process to learn DSA from scratch can be broken into 4 parts:
- Learn about Time and Space complexities
- Learn the basics of individual Data Structures
- Learn the basics of Algorithms
- Practice Problems on DSA

2）请把每个题目解题思路（可选），源码Python, 或者C++（已经在Codeforces/Openjudge上AC），截图（包含Accepted），填写到下面作业模版中（推荐使用 typora https://typoraio.cn ，或者用word）。AC 或者没有AC，都请标上每个题目大致花费时间。

3）提交时候先提交pdf文件，再把md或者doc文件上传到右侧“作业评论”。Canvas需要有同学清晰头像、提交文件有pdf、"作业评论"区有上传的md或者doc附件。

4）如果不能在截止前提交作业，请写明原因。



**编程环境**

操作系统：版本	Windows 11 家庭中文版
版本	22H2
安装日期	‎2023/‎7/‎18
操作系统版本	22621.2283
序列号	5CD323PJKL
体验	Windows Feature Experience Pack 1000.22662.1000.0

Python编程环境：* Spyder version: 5.4.3  (conda)

* Python version: 3.11.4 64-bit
* Qt version: 5.15.2
* PyQt5 version: 5.15.7
* Operating System: Windows 10

## 1. 题目

**02945: 拦截导弹**

http://cs101.openjudge.cn/practice/02945/



思路：



##### 代码

```python
k=int(input())
a=[int(i) for i in input().split()]
dp=[1]*k
for i in range(k):
    for j in range(i):
        if a[j]>=a[i] and dp[j]+1>dp[i]:
            dp[i]=dp[j]+1
print(max(dp))
```



代码运行截图 ==（至少包含有"Accepted"）==

![image-20240306172414853](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240306172414853.png)



**04147:汉诺塔问题(Tower of Hanoi)**

http://cs101.openjudge.cn/practice/04147



思路：



##### 代码

```python
def hanoi(k,a,b,c):#a现在的，b空的，c目标的
    if k==1:
        print("%d:%s->%s"%(k,a,c))
        return
    hanoi(k-1,a,c,b)
    print("%d:%s->%s"%(k,a,c))
    hanoi(k-1,b,a,c)


n,a0,b0,c0=input().split()
n=int(n)
hanoi(n,a0,b0,c0)
```



代码运行截图 ==（至少包含有"Accepted"）==

![image-20240306172447209](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240306172447209.png)



**03253: 约瑟夫问题No.2**

http://cs101.openjudge.cn/practice/03253



思路：



##### 代码

```python

n,p,m=map(int,input().split())
while n!=0:
    kid=[i for i in range(1,n+1)]
    ans=[]
    a=p-1
    while n>0:
        for i in range(m-1):
            if a==n:
                a=0
            a+=1
        if a==n:
            a=0
        #print(a)
        ans.append(kid[a])
        del kid[a]
        n-=1
        
    print(*ans,sep=',')
    n,p,m=map(int,input().split())

```



代码运行截图 ==（AC代码截图，至少包含有"Accepted"）==

![image-20240306172512474](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240306172512474.png)



**21554:排队做实验 (greedy)v0.2**

http://cs101.openjudge.cn/practice/21554



思路：



##### 代码

```python
n=int(input())
t=[int(i) for i in input().split()]
T=[]
for i in range(n):
    T.append([t[i],i+1])
T.sort()
ans=0
for i in range(n):
    ans+=T[i][0]*(n-i-1)
    print(T[i][1],end=' ')
print()
print("%.2f"%(ans/n))
```



代码运行截图 ==（AC代码截图，至少包含有"Accepted"）==

![image-20240306172539163](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240306172539163.png)



**19963:买学区房**

http://cs101.openjudge.cn/practice/19963



思路：



##### 代码

```python
import copy
n=int(input())  
pairs = [i[1:-1] for i in input().split()]
dis = [ sum(map(int,i.split(','))) for i in pairs]
price=[int(i) for i in input().split()]
kprice=copy.deepcopy(price)
k=[dis[i]/price[i] for i in range(n)]

k.sort()
kprice.sort()
if n%2==1:
    k1=k[n//2]
    k2=kprice[n//2]
if n%2==0:
    k1=(k[n//2-1]+k[n//2])/2
    k2=(kprice[n//2-1]+kprice[n//2])/2

ans=0
for i in range(n):
    if dis[i]/price[i]>k1 and price[i]<k2:
        ans+=1
print(ans)
```



代码运行截图 ==（AC代码截图，至少包含有"Accepted"）==

![image-20240306172618738](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240306172618738.png)



**27300: 模型整理**

http://cs101.openjudge.cn/practice/27300



思路：



##### 代码

```python
model={}
na=[]
n=int(input())
for i in range(n):
    name,num=input().split('-')
    if num[-1]=='M':
        numm=float(num[0:len(num)-1])
    else:
        numm=float(num[0:len(num)-1])*1000
    
    if model.get(name,0):
        model[name]=model[name]+[[numm,num]]
    else:
        model[name]=[[numm,num]]
        na.append(name)

na.sort()
for i in range(len(na)):
    print(na[i],end=": ")
    #print(model[na[i]])
    model[na[i]].sort()
    for j in range(len(model[na[i]])-1):
        print(model[na[i]][j][1],end=', ')
    print(model[na[i]][-1][1])
```



代码运行截图 ==（AC代码截图，至少包含有"Accepted"）==

![image-20240306172644235](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240306172644235.png)



## 2. 学习总结和收获

通过这次月考又回忆起了很多语法，例如字典，排序，格式化输出，递归，动规等





