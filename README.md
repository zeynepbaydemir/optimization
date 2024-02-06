# Optimizasyon Projesi
Bu proje, farklı arama algoritmalarını (genişletme öncelikli arama, derinlik öncelikli arama ve açgözlü arama) kullanarak bir labirentte başlangıç noktasından hedef noktasına ulaşmayı hedefler. Labirent, belirli boyutlarda rastgele oluşturulur ve bu labirentteki yol bulma algoritmaları performanslarını ölçer. Ayrıca, labirentteki engellerin ve taşların (ekstra zorluklar) algoritmanın çözüm süresine etkisini değerlendirir.

#### Projede yapılanlar:

- MazeSize sınıfı: Labirentlerin farklı boyutlarını belirler.
- Maze sınıfı: Labirenti oluşturur, engelleri ve taşları ekler.
- bfs, dfs ve greedy fonksiyonları: Sırasıyla genişletme öncelikli arama, derinlik öncelikli arama ve açgözlü arama algoritmalarını uygular.
- main fonksiyonu: Farklı boyutlardaki labirentler için algoritmaları test eder ve sonuçları raporlar.

Projede amaç, farklı arama algoritmalarının labirent problemini nasıl çözdüğünü anlamak, performanslarını karşılaştırmak ve labirentteki engeller ve taşlar gibi farklı koşulların algoritmaların çözüm süresi üzerindeki etkisini gözlemlemektir.

#### 1.	Proje Tanımı:
Bu proje, labirentlerin çeşitli kısıtlara göre oluşturulması ve çeşitli arama algoritmalarının(BFS, DFS, Greedy) bu labirentleri çözme sürelerinin ölçülmesi üzerine odaklanmaktadır. Labirentler farklı boyutlarda olabilir ve içerisinde belirli sayıda(15) taş bulunabilir ya da bulunmayabilir. Projede bulunan labirentler; 8x8, 12x12 ve 16x16 boyutlarından oluşmaktadır. Her bir boyutta labirentlerin taşlı ve taşsız durumu da karşılaştırılmıştır. Taşlı duruma göre algoritmamız yolu bulurken taşa takılırsa hızı 2 kat yavaşlıyor. Algoritmanın yolu bulurken geçirdiği süre de buna bağlı olarak artıyor. Proje, labirentlerin taşlı ve taşsız durumlarında çeşitli arama algoritmalarının performansını karşılaştırmayı amaçlamaktadır.


#### Problemin Tanımı:
1.	Labirentler, başlangıç ve hedef noktalarıyla birlikte belirli boyutlarda oluşturulur.
2.	Labirentlerde belirli sayıda taş ve engel bulunabilir.
3.	Proje, Breadth-First Search (BFS), Depth-First Search (DFS) ve henüz belirlenmemiş bir Greedy algoritması kullanarak labirentleri çözmeyi amaçlar.
4.	Her algoritmanın çözüm süresi, mikrosaniye cinsinden ölçülerek karşılaştırılır.
5.	Labirentin çözümü sırasında taşlara veya engellere takılma durumu kontrol edilir.
6.	Farklı labirent boyutları ve taşlı/taşsız durumlar için algoritmaların performansı karşılaştırılır.

#### Tartışma ve Sonuç
Bu projede, farklı boyutlarda ve taşlı/taşsız durumları içeren labirentler üzerinde Breadth-First Search (BFS), Depth-First Search (DFS) ve Greedy algoritmalarının performansı incelendi. Projenin temel sonuçları ve tartışma aşamaları şu şekildedir:

**Performans Karşılaştırması:**
- BFS, DFS ve Greedy algoritmalarının çözüm süreleri farklı labirent durumları için ölçüldü.
-	BFS, genellikle kısa sürelerde çözüm üretirken, DFS derinlemesine bir arama yaptığı için çözüm süreleri daha uzun olabilir.
-	Greedy algoritması için özel bir tasarım belirtilmemiş olsa da, genelde heuristik bir yaklaşım kullanıldığı düşünüldü.
  
**Taş ve Engellerin Etkisi:**
-	Labirentlere yerleştirilen taşlar ve engeller, algoritmaların performansını etkiledi.
-	Taşlı labirentlerde BFS ve DFS'nin performansında belirgin bir düşüş görüldü, çünkü bu algoritmalar taşlara çarptıklarında genellikle daha fazla adım atmaları gerekti.
-	Greedy algoritması, heuristik bir yaklaşım kullanarak taş ve engelleri daha etkili bir şekilde yönetebilir.
  
**Labirent Boyutunun Etkisi:**
-	Labirent boyutları arttıkça, algoritmaların çözüm süreleri genellikle arttı.
-	BFS ve DFS, büyük labirentlerde daha fazla adım atmaları gerektiği için daha fazla süre aldı.
-	Greedy algoritması, heuristik yaklaşımı sayesinde labirent boyutundan daha az etkilenmiş gibi görünüyor.
  
**Sonuçlar ve İlerleme:**
-	Proje, farklı durumlar için çeşitli algoritmaların performansını karşılaştırmak açısından önemli bilgiler sağladı.
-	Her algoritmanın avantajları ve dezavantajları belirlendi.
-	İleride yapılacak çalışmalarda, daha karmaşık algoritmaların ve heuristik yaklaşımların labirent çözümünde nasıl performans göstereceği incelenebilir.

