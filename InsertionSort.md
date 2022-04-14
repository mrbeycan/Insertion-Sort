# Insertion Sort

### Proje1

### [22,27,16,2,18,6] -> Insertion Sort

### - Yukarı verilen dizinin sort türüne göre aşamalarını yazınız

- 0.indexteki eleman ele alınır.
       - Dizideki diğer elemanlarla kıyaslanır ve dizinin en küçük elemanı 0. indeksteki elemanla yer değiştirir.
       - Dizi [2,27,16,22,18,6] olur.
- 1. indexteki  eleman ele alınır ve 0. indexteki eleman daha önce sıralandığı için kıyasa alınmaz ve dizide kalan diğer elemanlarla 1. indexteki eleman kıyaslanır ve en küçük elemanla 1. indexteki eleman yer değiştirir.
       - Dizi [2,6,16,22,18,27] olur.
- 2. indexteki  eleman ele alınır ve 0. ve 1. indexteki elemanlar daha önce sıralandığı için kıyasa alınmaz ve dizide kalan diğer elemanlarla 2. indexteki eleman kıyaslanır ve en küçük elemanla 2. indexteki eleman yer değiştirir. Eğer dizi kalan en küçük eleman kendisiyse hiç dokunulmaz ve sıradki diğer eleman ele alınır.
       - Dizi [2,6,16,22,18,27] olur.
- 3. indexteki  eleman ele alınır ve 0., 1. ve 2. indexteki elemanlar daha önce sıralandığı için kıyasa alınmaz ve dizide kalan diğer elemanlarla 3. indexteki eleman kıyaslanır ve en küçük elemanla 3. indexteki eleman yer değiştirir.
        - Dizi [2,6,16,18,22,27] olur.
- Dizimiz sıralanmış oldu biz bunu gözümüzle gördüğümüz için ayırt edebildik ve işlemi daha devam ettirme gereği duymadık fakat bilgisayarlar bunları kendiler anlayamadıkalrıiçin dizide n-1 eleman kalana kadar bu işlemi yapar ve  böylelikle dizi sıralı halinin getirilmiş olur.

-----------------------------
### Big-O gösterimini yazınız

- Insertion Sort algoritması sıralama yaparken her aşamada dizideki sıralanmamış bütün elemanları kıyaslıyor. 
- n tane elemanı olan bir dizide ilk aşamada n kere işlem yapıyor. ikinci aşamada n-1 tane ve dizide bir eleman kalana kadar bu işlem böyle devam ediyor.
- Big-O Notation için n+(n-1)+(n-2)...buda n ardışık sayının toplamı formülünden n*(n+1)/2 bu formülü açtığımınzda (n^2+2n+1)/2 gelir bu formülde baskın olan n^2 olduğu için Big-o Notation n^2 oluyor.

--------------------------------------------------------------------------------------------

### Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız

- Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.

- Burada da diziyi sıraladığımızda 18 sayısı dizinin orta kısmına denk geldiğini söyleyebilirz ve aradığımız sayı Worst Case kapsamına daha yakındır.
