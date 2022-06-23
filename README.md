```
$c = (curl -URI https://raw.githubusercontent.com/kalaxity/memory_exec_test/main/test.txt).content
$s = [scriptblock]::create($c)
$s.invoke()
```

もしくはそれらをまとめて一行で

```
([scriptblock]::create((curl -URI https://raw.githubusercontent.com/kalaxity/memory_exec_test/main/test.txt).content)).invoke()
```

## ref.
https://qiita.com/zaki-lknr/items/8950f6acea20961a8afc

https://yomon.hatenablog.com/entry/2014/11/27/222621
