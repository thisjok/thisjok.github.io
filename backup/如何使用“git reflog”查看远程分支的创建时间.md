使用reflog命令查看到指定分支的历次更改记录，最下面一条的时间即是分支创建时间：
```
$ git reflog show --date=iso origin/test_branch
```
```
6e9d15a9 (origin/release_r3.6.1) refs/remotes/origin/release_r3.6.1@{2024-03-20 18:54:07 +0800}: fetch: fast-forward
dc85df15 (release_r3.6.1) refs/remotes/origin/release_r3.6.1@{2024-03-20 15:15:04 +0800}: fetch: fast-forward
671f6b97 refs/remotes/origin/release_r3.6.1@{2024-03-12 15:24:49 +0800}: fetch: fast-forward
2d893a75 refs/remotes/origin/release_r3.6.1@{2024-03-06 14:32:28 +0800}: fetch: fast-forward
07fd91c8 refs/remotes/origin/release_r3.6.1@{2024-02-04 20:24:20 +0800}: fetch: fast-forward
a0a2eb93 refs/remotes/origin/release_r3.6.1@{2024-01-26 17:25:43 +0800}: fetch: fast-forward
3f28e740 refs/remotes/origin/release_r3.6.1@{2024-01-20 15:10:49 +0800}: fetch: fast-forward
108e5f02 refs/remotes/origin/release_r3.6.1@{2024-01-18 15:20:06 +0800}: fetch: fast-forward
76216323 refs/remotes/origin/release_r3.6.1@{2024-01-17 11:42:55 +0800}: fetch: fast-forward
dfb05954 refs/remotes/origin/release_r3.6.1@{2024-01-12 17:48:53 +0800}: fetch: fast-forward
e82f4312 refs/remotes/origin/release_r3.6.1@{2024-01-11 16:33:19 +0800}: fetch: fast-forward
47df2ac9 refs/remotes/origin/release_r3.6.1@{2024-01-09 11:24:09 +0800}: fetch: storing head
```