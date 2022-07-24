
 [patika.dev](https://www.patika.dev)



# Merge Sort Projesi
# Proje 2

### [16,21,11,8,12,22] -> Merge Sort
Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

	Step :Divide [16,21,11] [8,12,22] 
	Step :Divide [16,21] [11] [8,12] [22] 
	Step :Divide [16] [21] [11] [8] [12] [22]
	Step :Sorted trivially [16,21] [8,11] [12,22]
	Step :Merge  [8, 11, 16, 21] [12,22]
	Step :Sorted Array [8, 11, 12, 16, 21, 22]

### Big-O gösterimini yazınız: 

Burda Big – O gösterimini 2 etapta inceleyecegiz. Öncelikle bu dizinin bölümlenmesini birinci bölüm olarak ele alacagiz. 2. bölüm olarakta bölümlere ayrilan alt dizinlerin  siralanip tekrar dizilmesini inceleyecegiz. Burdan elde edilen  Big- O fonksiyonlarini birlestirip  dizin icin MergeSort  Big-O sunu elde edecegiz. 
	
	Step 1 Divide   n/2        n/2
	
	Step 2 Divide  n/4       n/4        n/4        n/4
	
	Step 3 Divide n/8    n/8     n/8   n/8   n/8    n/8    n/8    n/8
	
	Step n Divide  n/n    n/n   n/n  ………


Buraya kadar olan adimlarda  Big- O Natation 2^x= n  => x= (log⁡(2n))

n boyutundaki bir dizinin n parcaya bölünmesi O(log⁡ (n))  dir.

Bundan sonraki adimda  tüm alt dizilerin birleştirilmesi , O(n) zaman alır. Dolayisiyla O(n log⁡(n))dir.

Worst- Case = Listenin büyükten kücüge dizilmis bir sekilde

Best- Case = Listenin kücükten büyüge sirali verilmesi

Burda bizim icin fark etmiycek ne yazik ki biz mecburen bölme  ve tekrar birlestirme islemini yapacagiz . Dolayisiyla Timekomplex daima   O(n log⁡(n)) .

