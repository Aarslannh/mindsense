# MindSense – Duygu Analizli Yapay Zekâ Eğitim Platformu

MindSense, ilkokul, ortaokul ve lise öğrencilerinin yapay zekâ destekli sesli ve yazılı sohbetlerle ders çalışabildiği, aynı zamanda duygu analizine dayalı psikolojik destek sunan hibrit bir eğitim platformudur.

## Projenin Amacı
- Öğrencilerin bireysel ders çalışmasını kolaylaştırmak
- Duygusal farkındalık oluşturarak psikolojik destek sağlamak
- Okul rehberlik servislerine erken uyarı sistemi sunmak  
- Branş ve etüt öğretmenlerine öğrencilerin kazanım eksiklikleri hakkında veriler sunmak
## Hedef Kitle
- İlkokul, ortaokul ve lise öğrencileri  
- Rehber öğretmenler ve psikolojik danışmanlar
- Branş ve etüt öğretmenleri 
- Eğitim kurumları ve EdTech geliştiricileri  

---

## Ana Özellikler
| Modül                        | İşlevi |
|------------------------------|--------|
| Ders Seçimi Sistemi       | Öğrencinin çalışmak istediği dersi seçmesi |
| Sohbetli Eğitim Modülü    | Yapay zekâ ile yazılı ve sesli etkileşim |
| Duygu Analizi Sistemi     | Yanıtlardan duygu durumunu analiz etme |
| Sesli Giriş/Çıkış         | Sesli yanıt alma ve yanıtlama özelliği |
| Destek & Uyarı Mekanizması | Moral verici mesajlar veya rehberlik uyarısı |
| Rehberlik Paneli        | Rehber öğretmenler için bildirim paneli |

---

## Teknik Mimarisi
1. **Öğrenci:** Ders seçer → Yazılı/sesli cevap verir
2. **Speech-to-Text:** Whisper/Vosk ile ses metne çevrilir
3. **LLM:** Gemma / Gemini modeliyle AI yanıtı üretilir
4. **Duygu Analizi:** HuggingFace DistilBERT ile duygu tespiti yapılır
5. **Karar Mantığı:**  
   - Normal → Sohbet devam  
   - Hafif negatif → Destek mesajı  
   - Kritik → Rehber öğretmene uyarı  
6. **Veritabanı:** Supabase / MongoDB kayıt işlemleri  
7. **Rehber Paneli:** Uyarılar rehber öğretmene iletilir

---

## Kullanılan Teknolojiler
| Alan         | Teknoloji                                 | Kullanım Amacı                     |
|--------------|-------------------------------------------|------------------------------------|
| LLM          | Ollama Gemma 3B, Google Gemini Pro         | Eğitim diyaloğu, destek mesajları  |
| Ses Tanıma   | Whisper / Vosk                             | Sesin metne dönüştürülmesi         |
| TTS          | gTTS / Tortoise TTS                        | AI yanıtlarının seslendirilmesi    |
| Duygu Analizi| DistilBERT Emotion (HuggingFace)           | Duygu sınıflandırma                 |
| Arayüz       | Streamlit                                  | Web arayüzü                        |
| Veritabanı   | Supabase / MongoDB Atlas                   | Kullanıcı verileri & rehberlik     |
| Bildirim     | E-posta / Panel Uyarısı                    | Rehber uyarıları                    |

---

## Sprint Backlog
### Sprint 1 (2–5 Temmuz)
- Arayüz taslağı (wireframe)
- Ders seçme ekranı
- Yazılı chat + AI yanıtı prototipi
- Sesli giriş/çıkış testleri
- README ve görev dağılımı

### Sprint 2 (6–14 Temmuz)
- Duygu Analizi entegrasyonu
- Duyguya göre destek mesajları
- Ciddi durum sınıflandırması
- Uyarı prototipi (popup/email)
- Chat UI iyileştirmeleri

### Sprint 3 (15–22 Temmuz)
- Veritabanı entegrasyonu
- Rehberlik paneli geliştirme
- Demo videosu & sunum hazırlığı

---

## Örnek Kullanım Senaryosu
> Zeynep isimli öğrenci, Türkçe dersi çalışırken "başaramayacağım, çok yoruldum" gibi ifadeler kullanır.  
> Sistem, **kaygı ve üzüntü** tespit eder ve rehber öğretmene otomatik uyarı gönderir.  
> Rehber öğretmen panelden Zeynep’in durumunu görüntüleyip, gerekli müdahaleyi planlar.

---

## Projenin Katma Değeri
- Öğrencileri sadece akademik değil, duygusal yönden de destekler.
- Rehberlik ve yapay zekâ arasında köprü kurar.
- Erken müdahale sayesinde psikolojik riskleri azaltır.
- Hibrit (yazılı & sesli) öğrenme deneyimi sunar.

---

## Proje Ekibi
| İsim             | Rol            |
|------------------|----------------|
| Fatma Ceren Çil  | Scrum Master   |
| Seydi Dağlı      | Takım Üyesi    |
| Yusuf Tetik      | Takım Üyesi    |
| Aybüke Yıldız    | Takım Üyesi    |
| Hamide Arslan    | Product Owner  |

---

## Not
Bu proje, sosyal etki odaklı, açık kaynak bir eğitim teknolojisi uygulamasıdır.

---


