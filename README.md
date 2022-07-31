# Insertion-Sort-Projesi
[10,27,16,3,18,6] -> Insertion Sort
1.Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.
[10,27,16,3,18,6] -- (n)
açıklama:
Amacımız en küçük elemanı en başa getirmektir.Bu nedenle,mevcut ilk eleman ile en küçük elemanı yer değiştirmemiz gerekmektedir.Yani 3 başa geçer ve 10 ile yer değiştirir

3 elemanı,dizinin en başına yazılır ve 10 elemanı da,3 elemanının eski yerine yerleştirilir,yani elemanlar yer değiştirirler.Böylece 1.adım tamamlanmış olur.

1.ADIM:
[3,27,16,10,18,6] -- (n-1)

açıklama:
Daha sonra ise,ilk eleman(3) sabit tutulur ve 3.elemanın en küçük olacağı,diziyi büyükten küçüğe sıralayabileceğimiz diğer eleman aranır. [27,16,22,18,6] dizisindeki en küçük eleman 6 olduğu için,6 elemanı 2.eleman olarak seçilir ve mevcut 2.eleman ile (27), 6 elemanı yer değiştirir. 2.adım da bu şekilde tamamlanır.

2.ADIM:
[2,6,16,22,18,27] -- (n-2)

açıklama:
Aynı yol ile,dizideki elemanlar soldan sağa,büyükten küçüğe sıralanacak şekilde seçilmeye devam edilir.16'dan sonraki en büyük eleman 18 olduğundan, sıralamayı düzeltmek için 2.adımdaki 22 ile 18 yer değiştirir.Böylece 3.adım tamamlanmış olur.

3.ADIM:
[2,6,16,18,22,27] -- (n-3)

2.Big-O gösterimini yazınız.
O(n^2)'dir.
açıklama:
n + (n-1) + (n-2) + (n-3) + ... + 1 (Ardışık sayıların toplamı formülü) ve n.(n+1)/2 => n^2+n /2 'dir.
Big-O'da domine eden fonksiyon alınır,burada n^2 domine eden fonksiyon olduğu için,cevap O(n^2)'dir.

3.Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
Worst Case:
[27,22,18,16,6,2] - O(n^2)

Best Case:
[2,6,16,18,22,27] - O(n)

Average Case:
[2,6,16,18,22,27] - O(n^2) (Dizimizin son durumu zaten avarage case'e örnektir.)

4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
18 sayısı dizinin ortanca değeri olduğu için,avarage case kapsamına girmektedir.


[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
1.adım :
[2,3,5,8,7,9,4,15,6]
2.adım :
[2,3,4,8,7,9,5,15,6]
3.adım :
[2,3,4,5,7,9,8,15,6]
4.adım :
[2,3,4,5,6,9,8,15,7]
