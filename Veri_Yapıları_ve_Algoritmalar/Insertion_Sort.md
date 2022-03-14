## Proje_1 - Insertion Sort

**[22,27,16,2,18,6] -> Insertion Sort**

1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

```
[22,27,16,2,18,6] --> n
[2|,27,16,22,18,6] --> n-1
[2,6|,16,22,18,27] --> n-2 (16 en küçük olduğu için değişmiyor)
[2,6,16|,22,18,27] --> n-3
[2,6,16,18,22,27] --> 1
```
2. Big-O gösterimini yazınız.

```
n + (n-1) + (n-2) + ... + 1 (1'den n'e kadar olan sayıların toplamını veriyor.)
1'den n'e kadar olan sayıların toplamı: (n*(n+1))/2 = (n^2 +n) / 2 
**Dominant olan n^2 dolayısıyla big o notation gösterimi O(n^2)**
```
3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.

```
*Worst Case* O(n^2)

*Average Case* O(n^2)

*Best Case* O(n)
```

4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.

```
Dizi sıralandıktan sonraki hali: [2,6,16,18,22,27] 
Average Case kapsamına girer.
```

**[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.**

```

[7,3,5,8,2,9,4,15,6] --> n

[2|,3,5,8,7,9,4,15,6] --> n-1 
[2,3|,5,8,7,9,4,15,6] --> n-2 (3 en küçük olduğu için yerinde kalır.)
[2,3,4|,8,7,9,5,15,6] --> n-3
[2,3,4,5|,7,9,8,15,6] --> n-4

```