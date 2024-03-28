1. 使用命令(其中dev1-r350为本地创建的分支)

>  git reflog show  --date=local --all | grep dev1-r350

2. 命令输出
~~~
c470a67 HEAD@{Fri Aug 25 10:52:19 2023}: checkout: moving from release_r3.5-xyu to dev1-r350
9e0884f refs/remotes/origin/dev1-r350@{Fri Aug 25 10:24:12 2023}: fetch: fast-forward
7bd1877 HEAD@{Thu Aug 24 21:04:01 2023}: checkout: moving from dev1-r350 to origin/release_r3.5
c470a67 refs/heads/dev1-r350@{Thu Aug 24 17:56:06 2023}: branch: Created from HEAD
c470a67 HEAD@{Thu Aug 24 17:56:06 2023}: checkout: moving from c470a67eaba685adc4adaa9ad10d3dfb05fe2f5b to dev1-r350
c470a67 HEAD@{Thu Aug 24 17:44:53 2023}: checkout: moving from release_r3.5 to origin/dev1-r350
c470a67 refs/remotes/origin/dev1-r350@{Tue Aug 22 17:12:28 2023}: fetch: fast-forward
~~~

3. 输出数据分析
> 从倒数第2行及倒数第4行的reflog可以推断出：dev1-r350创建自origin/dev1-r350分支的commit ID为c470a67的节点；