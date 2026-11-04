JARVIS + Friday projem için, uygulamayı ilk kez kullanacak kişilere yönelik bir indirme, kurulum ve kullanım rehberi hazırla. Çıktı GitHub README dosyasında kullanılabilecek Markdown biçiminde olsun. Önce Türkçe, ardından İngilizce sürümünü yaz. Teknik bilgisi olmayan birinin takip edebileceği açık ve numaralı adımlar kullan.

Proje bilgileri:
- Geliştirici/yayıncı: DERİN DEVLET.
- Uygulama: Windows 64 bit için JARVIS + Friday masaüstü asistanı.
- Güncel sürüm: 2026.11.04.2.
- Gemini tam kurulum dosyası: JARVIS_Gemini_Hafif_Tam_Kurulum_2026-11-04_v16.exe
- Alternatif Ollama tam kurulumu: JARVIS_Ollama_Hafif_Tam_Kurulum_2026-11-04_v33.exe
- İndirme bağlantısı: [GITHUB RELEASES BAĞLANTISINI BURAYA EKLE]
- Her kurulum JARVIS ve Friday’i birlikte içerir. Kullanıcı tercih ettiği sürümü seçer; ikisini birden kurması gerekmez.
- Bunlar tam kurulumdur; önceki kurulum veya ayrıca Python kurulumu gerekmez.
- Gemini sürümü için Ollama gerekmez. İnternet ve kullanıcının kendi Gemini API anahtarı gerekir.
- Ollama sürümü yerel yanıtlar için kurulu Ollama modeli kullanır. Mevcut seslendirme ise Gemini bağlantısı gerektirir.

Rehberde şu konuları anlat:

1. İndirme ve kurulum
GitHub deposundaki Releases bölümünden doğru tam kurulum EXE’sinin seçilmesini, indirilmesini, çalıştırılmasını ve masaüstü kısayolundan uygulamanın açılmasını açıkla. Kaynak kod ZIP dosyasını kurulum dosyasıyla karıştırma. İndirme bağlantısı verilmemişse bağlantı uydurma; yer tutucuyu koru.
Resmî başvuru: https://docs.github.com/en/repositories/releasing-projects-on-github/viewing-your-repositorys-releases-and-tags

2. Gemini’yi ilk kez bağlama
Google AI Studio’dan kişisel API anahtarı edinme sürecini anlat:
https://aistudio.google.com/apikey
Kullanıcı uygulamada AYARLAR → GENEL → GEMINI BAĞLANTISI bölümüne girer. Anahtarını ilgili alana ekler, Google’a veri gönderimi açıklamasını okuyup onaylar ve GEMINI AYARLARINI KAYDET düğmesine basar. Gerçek bir anahtar isteme, örnek anahtar üretme veya anahtarın GitHub’da paylaşılmasını önerme.
Resmî başvuru: https://ai.google.dev/gemini-api/docs/api-key

3. İlk konuşma
Mesaj kutusuna yazarak GÖNDER düğmesiyle konuşmayı; mikrofon durumunu kontrol etmeyi; F5 ile mikrofonu duraklatıp sürdürmeyi anlat. F4 ses açma/kapatma içindir. CANLI düğmesiyle canlı konuşmanın kullanılabildiğini açıkla. AI MODELLERİ bölümünden JARVIS ve Friday arasında geçiş yapılabilir. Varsayılan sesler JARVIS için Charon, Friday için Kore’dir.

4. Kullanım örnekleri
Kısa açıklamalarıyla şu örnekleri ver:
- “Merhaba, nasılsın?”
- “Not al yarın projeye devam et.”
- “Günlük rapor.”
- “Kayıtlarımda ESP32 ara.”
- “Rutin merkezini aç.”
- “Verilerimi yedekle.”

FOTOĞRAF düğmesiyle görsel, BELGE düğmesiyle PDF/metin dosyası eklenebildiğini; EKRAN menüsüyle ekran hakkında soru sorulabildiğini anlat. Günlük raporda Gmail bilgisi için hesabın ayrıca AYARLAR → RAPOR / GMAIL bölümünden bağlanması gerektiğini belirt.

5. Yeni rutin özelliği
Somut bir başlangıç örneği yaz:
“Rutin merkezini aç” → “25 DK DERS TASLAĞI” → adımları incele → KAYDET → “Ders çalışmaya başla rutinini başlat.”
Ders modunun Ayarlar → Bilgisayar tercihlerine bağlı olduğunu belirt. “Rutini durdur” yalnızca kalan adımları iptal eder; açılmış uygulamaları kapatmaz veya kurulmuş zamanlayıcıyı geri almaz.

6. Veri ve bağlantı bilgisi
Gemini’nin soruları, ilgili sohbet/hafıza bağlamını ve seçilen ekleri Google üzerinden işlediğini açıkla. Canlı modda açık mikrofonun sesi Google’a iletilir; uygulama arka plana geçince canlı bağlantı kapanır. Yerel kayıt aramasının sonuçları modele gönderilmez. Kişisel yedek dosyaları şifrelenmez; hesap anahtarlarını, ek dosyaları ve rutin tanımlarını içermez.

7. Kısa sorun giderme
Mikrofon kapalı olması, yanlış giriş aygıtı, Windows mikrofon izni, internet bağlantısı, geçersiz API anahtarı ve kullanım kotası için anlaşılır kontrol adımları ver. Güncel fiyat, kota veya model erişimi hakkında doğrulanmamış bilgi yazma.

Olmayan özellikleri, indirme bağlantılarını veya düğmeleri uydurma. “Tamamen çevrimdışı”, “sınırsız ücretsiz” veya “her bilgisayarda sorunsuz çalışır” gibi iddialar ekleme. Ücret/kota bilgisini Google’ın güncel koşullarına bağla. Gereksiz kod, terminal komutu ve geliştirici ayrıntıları kullanma. Sonuç doğrudan yayımlanabilecek bir kullanıcı rehberi olsun.

