# rev-list-fail
rev-list returns nonsense

``` bash
git log --format=%H > git-log
shuf git-log > git-log-shuf
git rev-list --no-walk $(< git-log-shuf) > git-rev-list
diff git-log git-rev-list
```
