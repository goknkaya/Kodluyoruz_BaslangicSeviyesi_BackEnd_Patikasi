# Data Structures and Algorithms Projects

 Patika.dev Baslangic Seviye Back End Patikasi derslerinden Veri Yapilari ve Algoritmalar dersi odevleri

## Project 1 - Selection Sort Projesi

- [22, 27, 16, 2, 18, 6] -> Insertion Sort

Yukarıda gösterilen dizinin sort türüne göre aşamalarını yazın. Big-O gösterimini yazın.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case' lerden hangisinin kapsamına girer yazınız.

1) Average Case: Aradığımız sayının ortada olması
2) Worst Case: Aradığımız sayının sonda olması
3) Best Case: Aradığımız sayının en başlarda olması

#### Çözüm:

- [22, 27, 16, 2, 18, 6] -> En küçüğüne bak, en küçüğü 2, baştaki 22 ile yer değiştir. -> n
- [2, 27, 16, 22, 18, 6] -> 2 en başta ve hariç tutulacak şekilde en küçüğüne bak, en küçüğü 6, baştaki 27 ile yer değiştir. -> n-1
- [2, 6, 16, 22, 18, 27] -> 2 ve 6 en başta ve hariç tutulacak şekilde en küçüğüne bak, en küçüğü 16, en başta yer aldığı için yer değişikliğine gerek yok. -> n-2
- [2, 6, 16, 22, 18, 27] -> 2, 6 ve 16 en başta ve hariç tutulacak şekilde en küçüğüne bak, en küçüğü 18, baştaki 22 ile yer değiştir. -> n-3
- [2, 6, 16, 18, 22, 27] -> 2, 6, 16 ve 18 en başta ve hariç tutulacak şekilde en küçüğüne bak, en küçüğü 22, en başta yer aldığı için yer değişikliğine gerek yok. -> n-4
- [2, 6, 16, 18, 22, 27] -> Dizinin en son hali bu sekilde olmalidir. -> 1

#### Big-O Notation:

n + (n-1) + (n-2) + (n-3) + (n-4) + 1 -----> (n * (n+1)) / 2 -----> (n^2) * n / 2 -----> O(n^2)

#### Time Complexity:

[2, 6, 16, 18, 22, 27] -> Dizi sıralı haliyle bu şekildedir. 2 -> Lower, 27 -> Higher ve 18 -> Middle' dir. Dolayısıyla 18 average case kapsamındadır.

-----------------------------------------------------------------------------------

- [7, 3, 5, 8, 2, 9, 4, 15, 6] dizisinin Selection Sort' a göre ilk dört adımını yazınız:

  #### Çözüm:

  - Step 0 -> [7, 3, 5, 8, 2, 9, 4, 15, 6] -> Tüm dizi tarandı, en küçük eleman 2, en baştaki 7 ile yer değişti ve aşağıdaki gibi oldu.
  - Step 1 -> [2, 3, 5, 8, 7, 9, 4, 15, 6] -> En baştaki eleman 2 hariç tutuldu, dizinin en küçük elemanı 3, en başta bulunduğu için yer değiştirmedi.
  - Step 2 -> [2, 3, 5, 8, 7, 9, 4, 15, 6] -> En baştaki elemanlar 2 ve 3 hariç tutuldu, dizinin en küçük elemanı 4, en baştaki 5 ile yer değiştirdi ve aşağıdaki gibi oldu.
  - Step 3 -> [2, 3, 4, 8, 7, 9, 5, 15, 6] -> En baştaki elemanlar 2, 3 ve 4 hariç tutuldu, dizinin en küçük elemanı 5, en baştaki 8 ile yer değiştirdi ve aşağıdaki gibi oldu.
  - Step 4 -> [2, 3, 4, 5, 7, 9, 8, 15, 6] -> En baştaki elemanlar 2, 3, 4 ve 5 hariç tutuldu, dizinin en küçük elemanı 6, en baştaki 7 ile yer değiştirdi ve aşağıdaki gibi oldu.
  - Step 5 -> [2, 3, 4, 5, 6, 9, 8, 15, 7] -> En baştaki elemanlar 2, 3, 4, 5 ve 6 hariç tutuldu, dizinin en küçük elemanı 7, en baştaki 9 ile yer değiştirdi ve aşağıdaki gibi oldu.
  - Step 6 -> [2, 3, 4, 5, 6, 7, 8, 15, 9] -> En baştaki elemanlar 2, 3, 4, 5, 6 ve 7 hariç tutuldu, dizinin en küçük elemanı 8, en başta bulunduğu için yer değiştirmedi.
  - Step 7 -> [2, 3, 4, 5, 6, 7, 8, 15, 9] -> En baştaki elemanlar 2, 3, 4, 5, 6, 7 ve 8 hariç tutuldu, dizinin en küçük elemanı 9, en başta bulunan 15 ile yer değiştirdi ve aşağıdaki gibi oldu.
  - Step 8 -> [2, 3, 4, 5, 6, 7, 8, 9, 15] -> Tüm elemanlar sıralanmış halde, dizinin son hali bu şekildedir.

 ## Project 2 - Merge Sort Projesi

- [16, 21, 11, 8, 12, 22] dizisinin sort türüne göre aşamalarını yazınız. Big-O gösterimini yapınız.

#### Çözüm:

![Proje2](https://i.hizliresim.com/hpdyxqv.png)

## Project 3 - Binary Search Tree Projesi

![Proje3](https://i.hizliresim.com/dlgs7gw.png)

- Step 1: 1<5 için Root' un solunda 1
- Step 2: 7>5 için Root' un sağında 7
- Step 3: 0<1 ve 0<5 için Root' un solunda 0
- Step 4: 3>1 ve 3<5 için Root' un sağında 3
- Step 5: 2<3, 2>1 ve 2<5 için Root' un solunda 2
- Step 6: 4>3, 4>1 ve 4<5 için Root' un sağında 4
- Step 7: 6<7 ve 6>5 için Root' un solunda 6
- Step 8: 9>7 ve 9>5 için Root' un sağında 9
- Step 9: 8<9 ve 8>5 için Root' un solunda 8
