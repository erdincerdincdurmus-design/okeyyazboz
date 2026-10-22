# Yazboz Master Pro+

Okey oyunu için geliştirilmiş, telefonda kullanıma uygun **puan tablosu ve hesap bölüşüm uygulaması**. Tek bir `index.html` dosyasından oluşur, dış kütüphane ya da internet bağlantısı gerektirmez.

**Canlı sürüm:** `https://erdincerdincdurmus-design.github.io/okeyyazboz/`

## Neler yapar?

### PUAN sekmesi
- 4 oyuncu, 11 el için puan tablosu. Oyuncu isimleri tablo başlığına yazılır.
- **Hızlı ödül girişi:** Kazananın cezası tek dokunuşla girilir (-40 kırmızı, -50 siyah, -60 sarı, -70 mavi).
- **Çarpan düğmeleri (4x-7x):** Diğer oyuncuların elindeki sayılar renk çarpanıyla çarpılır ve satır kilitlenir. Çarpmadan önce dört kutunun da dolu olması gerekir.
- **Okey atıldı / Çift bitti:** Kazananın ödülü okeyde 10 katına, çiftte 20 katına çıkar (örneğin kırmızıda -400 / -800). Diğer oyuncuların sayıları renk çarpanının iki katıyla çarpılır (8, 10, 12, 14).
- **Taş yapma sırası:** İlk taş yapan oyuncu seçilir, sonraki ellerde sıra her satırda bir sonraki oyuncuya geçer ve kutu çerçevesiyle gösterilir.
- **Renkli genel toplam:** En az ceza yeşil, ikinci sarı, üçüncü açık kırmızı, en kötü koyu kırmızıdır.
- **Yan çevirme görünümü:** Telefon yan çevrilince toplamlar ekranı kaplayan büyük kutularda görünür. Kırmızı oyuncuların altında, sarıya olan puan farkı küçük etiketlerle anlık olarak gösterilir. En kötü oyuncuda açık kırmızıya olan fark da görünür.

### HESAP sekmesi
- Ürünler **fiyat × adet** şeklinde girilir (örneğin `20 × 8 = 160`), toplam hesap otomatik hesaplanır.
- Oynanan parti sayısı ve oyuncuların yenilgi sayıları girilince her oyuncunun hissesi ve ödeyeceği tutar hesaplanır. Pay, oyuncunun yenilgisinin toplam yenilgiye oranıdır (3 partide 3/6, 2/6, 1/6 gibi).
- **11. el bitince** parti sayısı otomatik artar ve en çok ceza alan iki oyuncunun yenilgi sayısı otomatik yazılır. İkinci en kötü puanda eşitlik varsa eşit olan herkes yenilmiş sayılır.

### Kayıt ve silme
- Puanlar, isimler ve hesap cihazda saklanır, uygulama kapansa da kaybolmaz.
- Üç ayrı silme düğmesi vardır: **SİL** (sadece puanlar), **HESABI SIFIRLA** (ürünler, parti ve yenilgi sayıları) ve **İSİMLERİ SİL**.

## Nasıl kullanılır?

**iPhone:** Canlı sürüm bağlantısını Safari'de açın, **Paylaş → Ana Ekrana Ekle** deyin ve uygulamayı ana ekrandaki simgeden kullanın.

**Android:** Aynı bağlantı Chrome'da da açılır. Dosya ayrıca MIT App Inventor ile Android uygulamasına çevrilerek de kullanılabilir.

## Teknik notlar
- Tek dosya (`index.html`), saf HTML, CSS ve JavaScript.
- Veriler sunucuya gönderilmez, yalnızca cihazın kendi depolamasında tutulur.
- `icon.png`, iPhone ana ekran simgesi olarak kullanılır.
