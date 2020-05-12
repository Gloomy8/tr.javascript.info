
```js no-beautify
"" + 1 + 0 = "10" // (1)
"" - 1 + 0 = -1 // (2)
true + false = 1
6 / "3" = 2
"2" * "3" = 6
4 + 5 + "px" = "9px"
"$" + 4 + 5 = "$45"
"4" - 2 = 2
"4px" - 2 = NaN
7 / 0 = Sonsuz
" -9  " + 5 = " -9  5" // (3)
" -9  " - 5 = -14 // (4)
null + 1 = 1 // (5)
undefined + 1 = NaN // (6)
```

1. String ile toplamada (`"" + 1`) , `1` sayısı string olarak dönüştürülür: `"" + 1 = "1"`, ve sonrasında `"1" + 0` için de aynı kural uygulanır.
2. Sting ile çıkarmada `-` (çoğu matematik işleminde olduğu gibi) sadece sayılarla çalışılır, boş bir string'i (`""`) , `0` olarak dönüştürür.
3. String ile toplama `5` sayısını da string'e çevirir.
4. Çıkarma işlemi her zaman sayıya dönüştürür, yani `"  -9  "` string'ini `-9` olarak dönüştürür (etrafındaki boşlukları görmezden gelir).
5. `null` , sayısal dönüşümden sonra `0` değerini alır.
6. `undefined` , sayısal dönüşümden sonra `NaN` değerini alır.
