# 🎭 Yüz ve Duygu Tanıma Uygulaması (Vue + face-api.js)

Bu proje, tarayıcı üzerinden gerçek zamanlı **yüz algılama** ve **duygu tanıma** işlemlerini yapar. Vue 3 ve face-api.js kullanılarak geliştirilmiştir.

---

## 🚀 Özellikler

- ✅ Gerçek zamanlı yüz tespiti
- 😊 7 temel duygu analizi:
  - `neutral`, `happy`, `sad`, `angry`, `fearful`, `disgusted`, `surprised`
- 🧠 TensorFlow.js destekli yapay zeka modeli
- 🌐 Tarayıcıda çalışır, backend gerekmez

---

## 🛠️ Kullanılan Teknolojiler

- [Vue 3 (CDN)](https://vuejs.org/)
- [face-api.js](https://github.com/justadudewhohacks/face-api.js)
- WebRTC (kamera erişimi)
- Canvas API (görsel çizim)

---

## 📁 Kurulum

1. Bu projeyi bilgisayarınıza indirin veya klonlayın:
    ```bash
    git clone https://github.com/kullanici/vue-face-emotion.git
    cd vue-face-emotion
    ```

2. `index.html` (veya `selam.html`) dosyasının bulunduğu dizine şu yapıda bir klasör oluşturun:

    ```
    .
    ├── selam.html
    └── models/
        ├── tiny_face_detector_model-weights_manifest.json
        ├── tiny_face_detector_model-shard1
        ├── face_expression_model-weights_manifest.json
        └── face_expression_model-shard1
    ```

3. Gerekli model dosyalarını buradan indir:
    - [`tiny_face_detector_model`](https://github.com/justadudewhohacks/face-api.js-models/tree/master/tiny_face_detector_model)
    - [`face_expression_model`](https://github.com/justadudewhohacks/face-api.js-models/tree/master/face_expression_model)

---

## ▶️ Çalıştırma

1. `selam.html` dosyasını bir tarayıcıda aç (örneğin Chrome).
2. Kamera izni verdiğinizde, yüzünüz algılanır.
3. Alt kısımda duygu etiketi (`HAPPY`, `ANGRY`, vs.) görünür.

> 🎥 Web kamerası çalışmazsa tarayıcı izinlerini kontrol edin.

---

## 📸 Ekran Görüntüsü

![Ekran Görüntüsü](screenshots/preview.png)

> Alternatif olarak kendi ekran görüntünüzü `screenshots` klasörüne koyabilirsiniz.

---

## 📌 Geliştirme Notları

Bu yapı sadece `CDN` üzerinden çalışır. Build işlemi, Node.js kurulumu veya Webpack gerekmez. Sadece HTML + JS ile minimal bir test ortamı sunar.

İleri düzey kullanım için:
- Yüz verisiyle eşleştirme
- Fotoğraf üzerinden tanıma
- REST API ile kimlik doğrulama  
özellikleri de entegre edilebilir.

---

## 👨‍💻 Katkı Sağlamak

İyileştirme, yeni özellik veya hata düzeltmesi için PR'lar açabilirsiniz.  
Lütfen öncesinde bir `Issue` oluşturarak tartışalım.

---

## ⚖️ Lisans

MIT Lisansı © 2025  
Ferhat Cengiz ile birlikte geliştirildi.
