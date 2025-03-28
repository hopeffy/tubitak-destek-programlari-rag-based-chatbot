# TÜBİTAK Destek Programları İçin Akıllı Soru-Cevap Sistemi

Bu proje, yapay zekâ tabanlı Retrieval-Augmented Generation (RAG) yaklaşımını kullanarak, TÜBİTAK destek programları hakkında hızlı ve doğru bilgi sağlayan bir sohbet sistemi geliştirmeyi amaçlamaktadır. Kullanıcılar, TÜBİTAK’ın farklı destek programlarına yönelik sorularını sisteme yönelterek, ilgili programlarla ilgili ayrıntılı ve güncel bilgilere erişebilirler.

## Proje Özeti

Proje, TÜBİTAK 2209-A ve 2209-B projeleri özelinde, girişimciler, araştırmacılar ve akademisyenler için bilgiye erişimi hızlandırmayı hedeflemektedir. PDF ve dökümana dayalı bilgi çekme (RAG) yöntemiyle, kullanıcının sorduğu sorulara en uygun yanıtı üretir. Geleneksel doküman tarama sürecini hızlandırarak, kullanıcıların en doğru destek programına yönlendirilmesini sağlar.

## Amaç ve Kapsam

- **Hedef Kitle**:
  - Üniversite öğrencileri ve akademisyenler (Araştırma projeleri için destek arayanlar)
  - Girişimciler ve startup ekipleri (TÜBİTAK ve KOSGEB fonlarına başvurmak isteyenler)
  - Kamu kurumları ve özel sektör çalışanları (Ar-Ge destek programlarından yararlanmak isteyenler)

- **Beklenen Katkılar ve Sonuçlar**:
  - Kullanıcılar, uzun dökümanları okumak zorunda kalmadan ilgili TÜBİTAK destek programlarını hızlıca öğrenebilecek.
  - Destek programlarına başvurmak isteyen araştırmacılar ve girişimciler için zamandan tasarruf sağlayacak.
  - TÜBİTAK’ın sunduğu programlara yönelik farkındalığı artırarak daha fazla proje başvurusu yapılmasına olanak tanıyacak.

## Teknik Yapı

- **Veri Kaynağı**: TÜBİTAK destek programları ile ilgili PDF belgeleri ve resmi web sitesi içerikleri.
- **Doğal Dil İşleme (NLP)**: RAG (Retrieval-Augmented Generation) tabanlı bir model kullanılarak metin tabanlı bilgiye erişim.
- **Sohbet Arayüzü**: Kullanıcı dostu bir chatbot aracılığıyla etkileşim.
- **Makine Öğrenimi & Vektör Veritabanı**: Bilgileri anlamlandırmak ve doğru yanıtları getirmek için yapay zekâ destekli vektör tabanlı sorgulama.

## n8n Kullanım Talimatları

Bu projeyi n8n platformunda çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

1. **n8n'i Kurun**:
   - n8n'i kurmak için [n8n Kurulum Kılavuzuna](https://n8n.io/docs) göz atabilirsiniz.

2. **Proje Dosyasını İndirin**:
   - Bu projeyi GitHub'dan indirmeniz gerekiyor:
     ```bash
     git clone https://github.com/hopeffy/tubitak-destek-programlari-rag-based-chatbot
     ```

3. **n8n İş Akışını İmport Etme**:
   - GitHub'dan indirdiğiniz proje dosyasındaki `n8n_workflow.json` dosyasını n8n arayüzüne import edin:
     1. n8n arayüzüne gidin.
     2. Sol üst köşede yer alan **"Import"** butonuna tıklayın.
     3. İndirilen `Tubitak_Burslar_Chatbot(1).json` dosyasını seçin ve import işlemini tamamlayın.

4. **Veri Kaynağını Yükleyin**:
   - Projede kullanılan TÜBİTAK destek programları ile ilgili PDF dosyalarını ve diğer veri kaynaklarını n8n iş akışınızla uyumlu şekilde sağlayın.

5. **Model ve İş Akışını Çalıştırın**:
   - n8n iş akışınızı başlatmak için, **Workflow** sekmesinde **"Execute Workflow"** butonuna tıklayın.

## Katkıda Bulunma

Bu projeye katkıda bulunmak isterseniz, aşağıdaki adımları takip edebilirsiniz:

1. Fork yaparak kendi versiyonunuzu oluşturun.
2. Yeni özellikler ekleyin veya hataları düzeltin.
3. Pull request gönderin.

## Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.

---

Eğer proje hakkında sorularınız varsa veya katkıda bulunmak istiyorsanız, lütfen iletişime geçin.
