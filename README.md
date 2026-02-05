# Truth Predictor: Optimization Benchmark (GD, SGD, Adam)

Projenin amacı, verilen bir soru-cevap çiftinin doğruluğunu tahmin eden bir model eğitirken farklı 
optimizasyon algoritmalarının (Gradient Descent, SGD, Adam) performanslarını karşılaştırmaktır.

## Özellikler
- **Veri Seti:** LM Studio üzerinden `Turkish-Gemma-9B-T1` modeli ile üretilen 200 örnekli özgün veri seti.
- **Embedding:** Metinleri vektöre çevirmek için `turkish-e5-large` modeli kullanılmıştır.
- **Model:** Tek katmanlı, `tanh` aktivasyon fonksiyonlu PyTorch modeli.
- **Görselleştirme:** t-SNE ile optimizasyon yörüngeleri ve Epoch/Time/Loss grafikleri.

## Sonuçlar
- **Adam**, en hızlı yakınsayan yöntem olmuştur (~0.35 saniye).
- **SGD**, Adam'a göre daha stabil bir ilerleme kaydetmiş ancak daha uzun sürede (~5 saniye) benzer doğruluğa ulaşmıştır.
