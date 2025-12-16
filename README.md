# Genetik Algoritma ile Tarım Arazisinde Gübre ve Sulama Optimizasyonu

## 📋 Proje Hakkında

Bu proje, **Yapay Zeka Sistemleri** dersi kapsamında, Genetik Algoritma (GA) kullanarak tarım arazisinde gübre ve sulama miktarlarını optimize eden bir optimizasyon çözümüdür.

### Senaryo
Tarım arazisinde maksimum verim elde etmek için gübre ve sulama miktarlarının optimal değerlerini bulmak.

## 🎯 Optimizasyon Problemi

### Amaç Fonksiyonu (Maksimizasyon)
$$y = 10x_1 + 6x_2 - 0.5x_1^2 - 0.2x_2^2$$

### Değişkenler ve Sınırlar
- **x₁**: Gübre miktarı (kg/da) → [0, 50] (tam sayı)
- **x₂**: Sulama miktarı (L/da) → [0, 100] (tam sayı)

### Kısıtlar (Constraints)
- $x_1 + 0.1x_2 \leq 60$
- $x_2 \geq 20$

## 🚀 Kurulum

### Gereksinimler
- Python 3.7 veya üzeri
- Jupyter Notebook
- NumPy
- Matplotlib

### Kurulum Adımları

1. **Repository'yi klonlayın:**
   ```bash
   git clone https://github.com/kullanici/genetik_opti.git
   cd genetik_opti
   ```

2. **Gerekli kütüphaneleri yükleyin:**
   ```bash
   pip install numpy matplotlib jupyter
   ```

   veya `requirements.txt` kullanarak:
   ```bash
   pip install -r requirements.txt
   ```

3. **Jupyter Notebook'u başlatın:**
   ```bash
   jupyter notebook
   ```

4. **Notebook'u açın:**
   - `genetik_algoritma_tarim.ipynb` dosyasını açın
   - Tüm hücreleri sırayla çalıştırın (Kernel → Restart & Run All)

## 📖 Kullanım

### Notebook Yapısı

Notebook aşağıdaki bölümlerden oluşmaktadır:

1. **Problem Tanımı**: Optimizasyon probleminin matematiksel formülasyonu
2. **Kütüphaneler**: Gerekli Python kütüphanelerinin içe aktarılması
3. **Hiperparametreler**: GA parametrelerinin tanımlanması
4. **Amaç Fonksiyonu**: Verim hesaplama fonksiyonu
5. **Uygunluk Fonksiyonu**: Penalty metodu ile kısıt kontrolü
6. **GA Operatörleri**:
   - İlk Popülasyon Oluşturma
   - Turnuva Seçimi
   - Tek Noktalı Çaprazlama
   - Rastgele Üniform Mutasyon
7. **Ana GA Döngüsü**: Elitizm ile optimizasyon
8. **Görselleştirme**: En iyi uygunluk değerinin evrimi
9. **Sonuç Analizi**: Optimum çözüm ve kısıt kontrolü

### Parametreleri Değiştirme

Notebook içindeki hiperparametreleri değiştirerek farklı sonuçlar elde edebilirsiniz:

```python
N = 100          # Popülasyon Büyüklüğü
Gen = 100        # Maksimum İterasyon Sayısı
P_c = 0.8        # Çaprazlama Oranı
P_m = 0.05       # Mutasyon Oranı
M = 1000         # Penalty Katsayısı
```

## 📊 Sonuçlar

Notebook çalıştırıldığında:
- Her nesildeki en iyi uygunluk değerinin evrimini gösteren grafik
- Optimum gübre ve sulama miktarları
- Maksimum verim değeri
- Kısıtların sağlanıp sağlanmadığı kontrolü

## 🔧 Genetik Algoritma Özellikleri

- **Seçim**: Turnuva Seçimi (Tournament Selection)
- **Çaprazlama**: Tek Noktalı Çaprazlama (Single-Point Crossover)
- **Mutasyon**: Rastgele Üniform Mutasyon
- **Elitizm**: En iyi birey korunur
- **Kısıt Yönetimi**: Penalty Metodu

## 📝 Lisans

Bu proje eğitim amaçlıdır.

## 👤 Yazar

- **Ad Soyad**: [Öğrenci Adı]
- **Öğrenci No**: [Öğrenci Numarası]
- **Ders**: Yapay Zeka Sistemleri

## 📚 Referanslar

- Genetik Algoritmalar teorisi ve uygulamaları
- Optimizasyon problemleri ve kısıt yönetimi

## 🤝 Katkıda Bulunma

Bu bir öğrenci projesidir. Sorularınız veya önerileriniz için issue açabilirsiniz.

---

**Not**: Bu proje, Yapay Zeka Sistemleri dersi kapsamında hazırlanmıştır.

