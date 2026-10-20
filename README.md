# F.R.I.D.A.Y-Female-Replacement-Intelligent-Digital-Assistant-Youth-
Merhaba okuyucu,

JARVIS ve FRIDAY dünyasına hoş geldin! Bu rehberde uygulamayı nasıl indireceğini, kuracağını, kullanmaya başlayacağını ve Ollama bağlantısını nasıl hazırlayacağını öğrenebilirsin.

**1. İndirme ve kurulum**

JARVIS ve FRIDAY aynı kurulum paketinde bulunur. İkisi için ayrı ayrı dosya indirmene gerek yoktur.

İndirme bağlantısı: [JARVIS & FRIDAY İNDİRME BAĞLANTISI]

Dosyayı indirdikten sonra **setup.exe** kurulum dosyasını aç ve ekrandaki adımları takip et. Kurulum tamamlandığında JARVIS ve FRIDAY’ı içeren uygulamayı başlat.

**2. İlk kullanım**

Sesli komut kullanacaksan mikrofonunu bağla, çalıştığını kontrol et ve gerekli mikrofon iznini ver. Uygulamada ses, mikrofon veya dil ayarları bulunuyorsa bunları kendine göre düzenle.

Arayüzde asistan seçimi sunuluyorsa JARVIS veya FRIDAY’ı seçebilirsin. Asistanlar arasında geçiş yöntemi ve kullanılabilir özellikler sürümüne göre değişebilir.

Uygulamanın desteklediği özelliklere bağlı olarak şu tür isteklerde bulunabilirsin:

- “YouTube’u aç.”
- “Saat kaç?”
- “Benimle sohbet et.”
- “Bana kısa bir hikâye yaz.”
- “Bu konuyu daha kolay anlayacağım şekilde açıkla.”

Yazılı giriş destekleniyorsa isteklerini klavyeyle de gönderebilirsin.

**3. Ollama’nın kurulumu**

Ollama, desteklenen yapay zekâ modellerini bilgisayarında çalıştırmanı sağlar. JARVIS ve FRIDAY aynı pakette olsa da Ollama ayrıca kurulmalıdır; uygulamanın kurulum paketi Ollama’yı zaten kuruyorsa bu adımı tekrar yapmana gerek yoktur.

[Ollama’nın resmî Windows indirme sayfasını](https://ollama.com/download/windows) aç. Elle indirme seçeneğiyle **OllamaSetup.exe** dosyasını indir ve kurulumu tamamla. Ollama Windows’ta arka planda çalışabilir.

**4. Yapay zekâ modelini hazırlama**

Ollama kurulduktan sonra yeni bir PowerShell veya Komut İstemi penceresi aç. Örnek olarak Qwen3 4B modelini indirmek için şu komutu yaz:

```powershell
ollama pull qwen3:4b
```

İndirme tamamlandığında modeli test etmek için şu komutu çalıştır:

```powershell
ollama run qwen3:4b
```

Sohbet başladığında “Merhaba, benimle Türkçe konuş.” yazabilirsin. Bu örnek bir modeldir; uygulamanın belirli bir model gerektirmesi durumunda onun yönergelerini takip et.

**5. Uygulamayı Ollama’ya bağlama**

JARVIS ve FRIDAY uygulamasının Ollama bağlantı yönergelerini takip et. Bağlantı ayarlarında sunucu adresi ve model adı isteniyorsa standart yerel bağlantı için şu bilgileri kullan:

- Ollama sunucu adresi: `http://localhost:11434`
- Örnek model adı: `qwen3:4b`

Model adı, indirdiğin modelle aynı olmalıdır. Uygulama farklı bir API adresi biçimi istiyorsa kendi yönergesini esas al. Ollama’nın standart yerel API adresi yukarıdaki adrestir.

Ollama bağlantısı yapay zekâ yanıtları için kullanılır. Ses tanıma, sesli yanıt ve bilgisayarda işlem yapma özellikleri uygulamanın kendi desteğine bağlıdır.

**6. Sorun yaşarsan**

Mikrofon çalışmıyorsa seçili mikrofonu ve izinleri kontrol et. Ollama bağlantısı kurulamıyorsa Ollama’nın açık olduğundan emin ol.

Hello reader,

Welcome to the world of JARVIS and FRIDAY! This guide explains how to download the application, install it, start using your assistants, and prepare an Ollama connection.

**1. Download and installation**

JARVIS and FRIDAY are included in the same installation package. You do not need to download separate installers for each assistant.

Download link: [JARVIS & FRIDAY DOWNLOAD LINK]

After downloading the file, open **setup.exe** and follow the installation steps. Once installation finishes, launch the application containing JARVIS and FRIDAY.

**2. Getting started**

If you want to use voice commands, connect your microphone, check that it works, and grant the necessary microphone permission. Adjust any available audio, microphone, or language settings.

If the interface provides an assistant selector, choose JARVIS or FRIDAY. The switching method and available features may vary by version.

Depending on the features supported by your application, you can try requests such as:

- “Open YouTube.”
- “What time is it?”
- “Chat with me.”
- “Write me a short story.”
- “Explain this topic in simpler words.”

If text input is supported, you can also type your requests.

**3. Installing Ollama**

Ollama lets you run supported AI models on your computer. Although JARVIS and FRIDAY share one installation package, Ollama needs its own installation unless your application’s installer already includes and installs it.

Visit the [official Ollama download page for Windows](https://ollama.com/download/windows). Use the manual download option to get **OllamaSetup.exe**, then complete the installation. Ollama can run in the background on Windows.

**4. Preparing an AI model**

After installing Ollama, open a new PowerShell or Command Prompt window. To download the example Qwen3 4B model, enter:

```powershell
ollama pull qwen3:4b
```

Once the download finishes, test the model with:

```powershell
ollama run qwen3:4b
```

When the conversation starts, type “Hello, please speak English with me.” This is an example model; if your application requires a specific model, follow its instructions instead.

**5. Connecting the application to Ollama**

Follow the Ollama connection instructions provided by the JARVIS and FRIDAY application. If its settings ask for a server address and model name, use these values for a standard local connection:

- Ollama server address: `http://localhost:11434`
- Example model name: `qwen3:4b`

The model name must match the model you downloaded. If the application requires a different API address format, follow its instructions. The address above is Ollama’s standard local API address.

The Ollama connection provides AI responses. Speech recognition, spoken replies, and actions on your computer depend on features implemented by the application.

**6. Troubleshooting**

If your microphone does not work, check the selected input device and microphone permissions. If the Ollama connection fails, make sure Ollama is running.

Use `ollama ls` to view downloaded models. If the Ollama server is not running, start it with `ollama serve`. You do not need to start another server if one is already running.

Response speed depends on your hardware and selected model. If a large model runs slowly, try using a smaller one.
İndirilen modelleri görmek için `ollama ls` komutunu kullanabilirsin. Ollama sunucusu çalışmıyorsa `ollama serve` ile başlatabilirsin; zaten çalışıyorsa yeniden başlatman gerekmez.

Yanıt hızı bilgisayarının donanımına ve seçtiğin modele bağlıdır. Büyük modeller yavaş çalışıyorsa daha küçük bir model kullanmayı deneyebilirsin.
