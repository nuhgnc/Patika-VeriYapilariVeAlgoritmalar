### [ 22 , 27 , 16 , 2 , 18 , 6 ] örnek dizisi insertion sort olarak incelenmesi ;
#### 1. Sort türüne göre aşamaları :
```sql
  1.aşama = [ 2 , 27 , 16 , 22 , 18 , 6 ]
  2.aşama = [ 2 , 6 , 16 , 22 , 18 , 27 ]
  3.aşama = [ 2 , 6 , 16 , 18 , 22 , 27 ]
```

------------

#### 2. Örnek Dizin Big - O gösterimi ;
##### Insertion Sort'tun ilk adımında her index'i tek tek kontrol edip en küçüğü ile yer değiştirme mantığı olduğu için eleman sayısı (n) kadar işlem sağlamaktadır. Daha sonraki adımlarda işlem sayısı (n-1), (n-2) şeklinde azalarak gider.
```sql
  1.aşama = [ 2 , 27 , 16 , 22 , 18 , 6 ]  ( n )
  2.aşama = [ 2 , 6 , 16 , 22 , 18 , 27 ]  (n-1)
  3.aşama = [ 2 , 6 , 16 , 18 , 22 , 27 ]    1  
```
###### Bu yüzden Big O Notation, O(n²) olarak bulunur.

------------
#### 3.Time Complexity incelemesi ;
```sql
  Avarage Case :  O(n²)
  Worst   Case :  O(n²)
  Best  Case   :  O(n)
```
------------
#### 4. Dizi sıralı hale geldikten sonra 18 sayısı hangi case kapsamına girdiği hakkında inceleme ;
3.aşama = [ 2 , 6 , 16 , 18 , 22 , 27 ] dizisi ile sıralı hale gelmektedir.
18 sayısı orta sayı olduğu için Avarage Case kapsamında değerlendirilmektedir.

### 5. Ornek_Dizi = [7 , 3 , 5 , 8 , 2 , 9 , 4 , 15 , 6] dizisini insertion sort ' a göre sıralama adımlarının ilk 4 adımı : 
```sql
  1.adım = [ 2 , 3 , 5 , 8 , 7 , 9 , 4 , 15 , 6 ]
  2.adım = [ 2 , 3 , 4 , 8 , 7 , 9 , 5 , 15 , 6 ]
  3.adım = [ 2 , 3 , 4 , 5 , 7 , 9 , 8 , 15 , 6 ]
  4.adım = [ 2 , 3 , 4 , 5 , 6 , 9 , 8 , 15 , 7 ]
```