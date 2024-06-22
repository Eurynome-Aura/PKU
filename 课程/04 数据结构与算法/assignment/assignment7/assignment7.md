# Assignment #7: April 月考

Updated 1557 GMT+8 Apr 3, 2024

2024 spring, Complied by余汶青 生命科学学院



**说明：**

1）请把每个题目解题思路（可选），源码Python, 或者C++（已经在Codeforces/Openjudge上AC），截图（包含Accepted），填写到下面作业模版中（推荐使用 typora https://typoraio.cn ，或者用word）。AC 或者没有AC，都请标上每个题目大致花费时间。

2）提交时候先提交pdf文件，再把md或者doc文件上传到右侧“作业评论”。Canvas需要有同学清晰头像、提交文件有pdf、"作业评论"区有上传的md或者doc附件。

3）如果不能在截止前提交作业，请写明原因。



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

### 27706: 逐词倒放

http://cs101.openjudge.cn/practice/27706/



思路：



代码

```python
s=input().split()
s.reverse()
print(*s,sep=' ')

```



代码运行截图

![image-20240418163639044](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240418163639044.png)



### 27951: 机器翻译

http://cs101.openjudge.cn/practice/27951/



思路：



代码

```python
m,n=map(int,input().split())
s=[int(i) for i in input().split()]
q=[]
ans=0
for i in range(n):
    if s[i] in q:
        continue
    if len(q)>=m:
        q.pop(0)
    #print(s[i])
    q.append(s[i])
    ans+=1
print(ans)

```



代码运行截图 

![image-20240418164438081](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240418164438081.png)





### 27932: Less or Equal

http://cs101.openjudge.cn/practice/27932/



思路：



代码

```python
n,k=map(int,input().split())
s=[int(i) for i in input().split()]
s.sort()
if k==0:
    if s[0]!=1:
        print(1)
    else:
        print(-1)
elif n==k:
    print(s[-1])
else:
    if s[k-1]!=s[k]:
        print(s[k-1])
    else:
        print(-1)
    

```



代码运行截图

![image-20240418165651001](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240418165651001.png)





### 27948: FBI树

http://cs101.openjudge.cn/practice/27948/



思路：



代码

```python
class treenode():
    def __init__(self,key):
        self.left=None
        self.right=None
        self.key=key
    def printt(self):
        if self.left!=None:
            self.left.printt()
            self.right.printt()
        print(self.key,end='')
        
        
    
def build(s):
    node=None
    if '1' in s and '0' in s:
        node=treenode('F')
    elif '1' in s:
        node=treenode('I')
    elif '0' in s:
        node=treenode('B')
    if len(s)>1:
        node.left=build(s[0:len(s)//2])
        node.right=build(s[len(s)//2:])
    return node
        
n=int(input())
s=input()
root=build(s)
root.printt()

```



代码运行截图

![image-20240418205148209](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240418205148209.png)



### 27925: 小组队列

http://cs101.openjudge.cn/practice/27925/



思路：



代码

```python
t=int(input())
people={}
team={}
for i in range(t):
    a=[int(i) for i in input().split()]
    for j in a:
        people[j]=i
    team[i]=[]
queue=[]
sanke=[]
in_queue=[0]*t
s=input()
while s!='STOP':
    if s[0]=='E':
        a=int(s[8:])
        if a not in people:
            queue.append(a)
            sanke.append(a)
            s=input()
            continue
        tt=people[a]
        if in_queue[tt]:
            team[tt].append(a)
        else:
            queue.append(tt)
            team[tt].append(a)
            in_queue[tt]=1
    if s[0]=='D':
        a=queue[0]
        if a in sanke:
            print(a)
            queue.pop(0)
            s=input()
            continue
        print(team[a].pop(0))
        if len(team[a])==0:
            queue.pop(0)
            in_queue[a]=0
    s=input()

```



代码运行截图

![image-20240418212236432](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240418212236432.png)

### 27928: 遍历树

http://cs101.openjudge.cn/practice/27928/



思路：



代码

```python
def traverse(node):
    for i in tree[node]:
        if i!=node:
            traverse(i)
        else:
            print(node)
    
tree={}
n=int(input())
findroot=[1]*n
node=[]
for i in range(n):
    a=[int(i) for i in input().split()]
    for j in a:
        if j not in node:
            node.append(j)
        if j!=a[0]:
            findroot[node.index(j)]=0
    b=a[0]
    a.sort()
    tree[b]=a
root=node[findroot.index(1)]

traverse(root)

```



代码运行截图

![image-20240418212256084](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20240418212256084.png)



## 2. 学习总结和收获



终于把月考补上了

感觉比作业简单，但坑有点多



