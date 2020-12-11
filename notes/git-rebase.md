https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase



https://www.atlassian.com/git/tutorials/merging-vs-rebasing


Merge create `1da733`, a commit for merging into master

```git
commit 926f01bf47b9170623a281aecf936fb82520e886 (HEAD -> master, origin/master
)
Merge: ea3cf16 1da7333
Author: sumtsui <38915833+sumtsui@users.noreply.github.com>
Date:   Fri Dec 11 15:46:35 2020 +0800

    Merge pull request #4 from sumtsui/mybranch

    feat: try using merge instead of rebase

commit 1da73330eae58cb84cd8b7d0d94402af5a6218f3 (origin/mybranch)
Merge: 9ab1fcc ea3cf16
Author: sumtsui <38915833+sumtsui@users.noreply.github.com>
Date:   Fri Dec 11 15:46:18 2020 +0800

    Merge branch 'master' into mybranch

commit 9ab1fcc9fa9531cb65dad4268f5aecaaef7bf55d (mybranch)
Author: Sum Xu <v-suxu@expedia.com>
Date:   Fri Dec 11 15:44:20 2020 +0800

    feat: try using merge instead of rebase

commit ea3cf1662c40ba6bf6e09894ef7e2e26ff40f21d
Merge: b1319b3 a70bd2b
Author: sumtsui <38915833+sumtsui@users.noreply.github.com>
Date:   Fri Dec 11 15:43:40 2020 +0800

    Merge pull request #3 from sumtsui/someoneelse

    feat: faster again

commit a70bd2bf8d75f6d0f5274c5667485a7ba4378ac4 (origin/someoneelse, someoneelse)
Author: Sum Xu <v-suxu@expedia.com>
Date:   Fri Dec 11 15:42:28 2020 +0800

    feat: faster again
```

whereas rebase will not

```git
commit b1319b3461e58c8e60d20017fdb9227db8467b83
Merge: 607a0ba 3437494
Author: sumtsui <38915833+sumtsui@users.noreply.github.com>
Date:   Fri Dec 11 15:30:12 2020 +0800

    Merge pull request #2 from sumtsui/mybranch

    feat: some work I do on mybranch

commit 3437494a8c6992f9c1dc1d640da3949d727fafd8
Author: Sum Xu <v-suxu@expedia.com>
Date:   Fri Dec 11 15:06:26 2020 +0800

    feat: some work I do on mybranch

commit 607a0baa9f39a2031ddd2674f4d4c373d727e6fb
Merge: 76f2ebd 6894bae
Author: sumtsui <38915833+sumtsui@users.noreply.github.com>
Date:   Fri Dec 11 15:10:26 2020 +0800

    Merge pull request #1 from sumtsui/someoneElseBranch

    feat: i merge faster than you

commit 6894bae2c9953dbe32cd5dd315f820d77749c340 (origin/someoneElseBranch)
Author: Sum Xu <v-suxu@expedia.com>
Date:   Fri Dec 11 15:08:45 2020 +0800

    feat: i merge faster than you
```
