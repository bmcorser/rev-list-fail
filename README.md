# rev-list-fail
rev-list returns nonsense

``` bash
git rev-list --no-walk $(git log --format=%H | shuf)
```
