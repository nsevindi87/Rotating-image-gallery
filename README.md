# Rotating-image-gallery

https://nsevindi87.github.io/Rotating-image-gallery/


HEDEF: Fotograflarin 3 boyutlu dönmesini saglayan bir slyat olusturma

Sürec:
- Fotograflarin (span icinde img) ve butonlarin ayri ayri yer aldigi containerlar olusturulur.
- CSS de kullanilan yeni ögrenilen özellikler;
        - containera - transform-style: preserve-3d;
        - transform: perspective(1000px) rotateY(0deg);
- JS : 
    - Container - prev ve next butonlarina baglanti atma
    - butona tiklandiginda event atanir.
    - Atanan event; containerin style erisip transform özellik degistirilir.
    - Burada rotateY özellige disarida olusturulan degisken ile erisilerek + - 45 derecelik degisiklikler yapmasi saglanir.
    - Butona tiklandiginda ilk bas bu degisken + -45 deger alinir ve sonrasinda fonksiyona gönderilere her defasinda degiskenin 
    güncel bilgisi foksiyonun icine atanmasi saglanir.
    - Fonksiyonun icinde settimeout ile otomatik belli sürelerle dönmesi saglanir.
    - Ancak butona tiklandiginda bu otomatik sürenin cakismamasi yeninden baslamasi icin disaridan bir deger settimeout a atanir. 
    - cleartimeout() fonksiyonu icinde bu degisken buton tiklamasi icine eklenir.
    - Bu ekleme settimeout un süresini sifirlar.
    - Slaytin kendiliginden baslayabilmesi icin de fonksiyon haricen ayrica cagrilir. 
    
  setTimeout()
  clearTimeout()
  
