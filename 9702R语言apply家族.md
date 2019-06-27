#**R语言apply家族**
**apply()**

apply（m，dimcode，f，fargs）

* m是一个矩阵。
* dimcode是维度编号，取1则为对行应用函数，取2则为对列运用函数。
* f是函数
* fargs是f的可选参数集

```r
#老王耗子药的单价，单位（元/袋）
(price=list(year2014=36:33,year2015=32:35,year2016=30:27))
lapply(price, mean)#对列表(list)中的每个元素实施某种“相同的操作”Split-Apply-Combine
sapply(price,mean)#sapply尝试对结果进行简化
```

```r
mapply
#mapply()对多个list中相同位置的元素共同作用，也就是sapply(  )的多变量版本
#mapply，* 点乘，即相同位置相乘。
(income_quarter=mapply('*', price,amount))
(amount=list(year2014=rep(200,4),year2015=rep(100,4),year2016=rep(300,4)))
(income_quarter=mapply('*', price,amount))#mapply，点乘
```
