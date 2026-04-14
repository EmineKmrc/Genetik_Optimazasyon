# Genetik_Optimazasyon
📖 Problemin Tanımı
Yapay Zeka Sistemleri dersi kapsamında, Genetik Algoritma (GA) kullanılarak kısıtlı bir optimizasyon problemini çözmek amacıyla geliştirilmiştir.
Bu projede, bir lojistik firmasına ait akıllı depoda kullanılan raf sisteminin yüksekliği ve derinliği, belirli fiziksel kısıtlar altında genetik algoritma kullanılarak optimize edilmiştir.
Amaç, depo verimliliğini artırırken aynı zamanda alan ve maliyet kısıtlarına uygun bir raf yerleşimi elde etmektir.
Amaç fonksiyonu:f(x₁, x₂) = 4x₁ + 3x₂ − 0.5x₁x₂
Değişkenler: x₁: Raf yüksekliği (metre)
             x₂: Raf derinliği (metre)
Kısıtlar: 2 ≤ x₁ ≤ 6 
          1.5 ≤ x₂ ≤ 4
          x₁ + x₂ ≤ 8
Bu kısıtlar depo alanı ve fiziksel sınırları temsil etmektedir. Kısıtları ihlal eden çözümler, genetik algoritma içerisinde uygunluk değeri sıfır atanarak elenmiştir.
Uygunluk fonksiyonu, her bireyin amaç fonksiyonuna ne kadar iyi bir çözüm sunduğunu ölçmektedir.
Kısıtları ihlal eden bireylerin uygunluk değeri sıfır olarak atanmış, böylece bu bireylerin seçilme olasılığı azaltılmıştır.
⚙️ Genetik Algoritma Bileşenleri
Bu projede seçilim yöntemi olarak turnuva seçilimi kullanılmıştır.
Her seçilim işleminde popülasyondan rastgele belirli sayıda birey seçilir ve bu bireyler arasından uygunluk değeri en yüksek olan ebeveyn olarak belirlenir.
Turnuva seçilimi, kısıt içeren optimizasyon problemlerinde daha kararlı ve dengeli sonuçlar verdiği için tercih edilmiştir.
Çaprazlama işlemi ile iki ebeveyn bireyin genleri birleştirilerek yeni bireyler oluşturulmuştur. Bu sayede genetik çeşitlilik artırılmıştır.
Mutasyon işlemi, belirli bir olasılıkla gen değerlerinde küçük rastgele değişiklikler yaparak algoritmanın yerel maksimumlara takılmasını önler.(Gen çeşitliliği sağlanır)
📊 Optimizasyon Sonuçları
🚀 Kurulum ve Çalıştırma
Proje Python 3 ortamında, Jupyter Notebook ile çalıştırılmak üzere hazırlanmıştır.
1-)Repoyu klonlayın:
    git clone 

2-)Gerekli kütüphaneleri yükleyin:
    pip install -r requirements.txt    

3-)Notebook'u çalıştırın: genetik_optimizasyon.ipynb dosyasını açarak tüm hücreleri çalıştırınız.  
cd genetik_optimizasyonu_senaryo5
