# Gizlilik Politikası / Privacy Policy — THARP

| Parametre / Field | Değer / Value |
| :--- | :--- |
| **Uygulama Adı / Application Name** | THARP |
| **Package/Identity/Name** | `ALLAHVERDCAN.THARP` |
| **Package/Identity/Publisher** | `CN=80F86ABB-4ABB-4524-A032-0CE77FF05712` |
| **Package/Properties/PublisherDisplayName** | `ALLAHVERDİ CAN` |
| **Geliştirici & Yayıncı / Publisher** | ALLAHVERDİ CAN |
| **İletişim E-Posta / Contact Email** | `oguzyanardag@gmail.com` |
| **Yürürlük Tarihi / Effective Date** | 11 Kasım 2026 / November 11, 2026 |

---

## 1. TÜRKÇE — Gizlilik ve Kişisel Verilerin Korunması Politikası

### 1.1. Genel Bakış ve Temel İlke
**THARP** (“Uygulama”), `CN=80F86ABB-4ABB-4524-A032-0CE77FF05712` sertifikalı yayıncı **ALLAHVERDİ CAN** tarafından geliştirilmiş yerel (offline-first) bir Windows masaüstü ağ telemetrisi, canlı osiloskop, DNS hızlandırıcı ve süreç güvenlik kalkanıdır.

Bu politikanın temel ilkesi şudur: **THARP, kullanıcılarının hiçbir kişisel verisini, ağ trafiği içeriğini, ziyaret ettiği web sitelerini veya bilgisayarındaki süreç listesini toplamaz, kaydetmez, izlemez veya herhangi bir uzak sunucuya aktarmaz.**

### 1.2. Hangi Veriler Erişilir ve Nasıl Kullanılır?
Uygulama, temel işlevlerini yerine getirebilmek için Windows işletim sisteminin yerel uygulama programlama arayüzlerine (Win32 IP Helper `iphlpapi.dll`, `kernel32.dll`, `ntdll.dll`) erişir:
- **Ağ Soketleri (TCP/UDP):** Bilgisayarınızdaki etkin bağlantıların IP adresleri, portları ve protokol durumları anlık olarak listelenir.
- **Süreç Bilgileri:** Ağ bağlantısı açan süreçlerin PID numarası, dosya yolu, RAM kullanımı ve X.509 dijital imza durumu doğrulanır.
- **Bant Genişliği ve Adaptör Bilgileri:** Ağ kartlarının anlık indirme (RX) ve yükleme (TX) hızları canlı dalga formu olarak hesaplanır.
- **Yerel ARP Tablosu:** Yerel ağdaki çift MAC adresi çakışmaları (olası MITM saldırıları) taranır.

**ÖNEMLİ:** Bu verilerin tamamı **yalnızca o an bilgisayarınızın RAM belleğinde** işlenir. Uygulama kapatıldığında bellek temizlenir. Hiçbir telemetri veya günlük verisi dışarıya iletilmez.

### 1.3. Üçüncü Taraf SDK'lar, Reklam ve Analitik
- Uygulama içerisinde Google Analytics, Firebase, telemetry SDK'ları veya herhangi bir üçüncü taraf takip kodu **bulunmaz**.
- Uygulama içerisinde herhangi bir reklam modülü veya reklam kimliği (Advertising ID) izleyicisi **bulunmaz**.

### 1.4. Yerel Ayar Dosyaları
Kullanıcının dil seçimi (TR/EN), ses açma/kapama tercihi ve özel eklediği ping sunucuları gibi tercihler yalnızca kullanıcının kendi bilgisayarındaki yerel uygulama dizininde (`%LOCALAPPDATA%\ALLAHVERDCAN_THARP\tharp_settings.json`) saklanır. Bu dosya dışarıyla paylaşılmaz.

### 1.5. Kullanıcı Hakları ve İletişim
KVKK ve GDPR ilkeleri uyarınca veri toplanmadığı için sistemlerimizde saklanan bir kişisel veri kaydı bulunmamaktadır. Her türlü soru, geri bildirim veya güvenlik bildirimi için geliştirici ile doğrudan iletişime geçebilirsiniz:
- **Yayıncı / Publisher:** ALLAHVERDİ CAN (`CN=80F86ABB-4ABB-4524-A032-0CE77FF05712`)
- **E-Posta:** oguzyanardag@gmail.com

---

## 2. ENGLISH — Privacy & Data Protection Policy

### 2.1. Overview & Core Philosophy
**THARP** ("the Application") is an offline-first Windows desktop network socket telemetry, live bandwidth oscilloscope, DNS optimizer, and process security utility developed by publisher **ALLAHVERDİ CAN** (`CN=80F86ABB-4ABB-4524-A032-0CE77FF05712`).

Our foundational privacy commitment is simple: **THARP does not collect, store, transmit, track, or share any personal data, network payloads, browsing history, or running process lists with any external server or third party.**

### 2.2. What Data Is Accessed and How It Is Handled
To deliver its real-time diagnostic and security features, THARP interacts exclusively with local Windows Win32 APIs (Kernel IP Helper `iphlpapi.dll`, `kernel32.dll`, `ntdll.dll`):
- **Network Sockets (TCP/UDP):** Displays local and remote IP endpoints, port numbers, connection states, and standard service labels.
- **Process Information:** Resolves process identifiers (PIDs), binary file paths, live working set memory usage, and X.509 Authenticode certificate validation.
- **Throughput & Adapters:** Computes real-time download (RX) and upload (TX) throughput to render live hardware-accelerated waveforms.
- **Kernel ARP Table:** Inspects the local IPv4 neighbor cache to detect potential local network MITM/spoofing anomalies.

**ALL DIAGNOSTICS EXECUTE 100% LOCALLY IN RAM.** No network packets, socket logs, or hardware identifiers are ever uploaded, recorded remotely, or monetized.

### 2.3. Zero Third-Party Trackers, Telemetry, or Ads
- The Application contains **zero** third-party analytics SDKs, telemetry beacons, or crash reporters.
- The Application contains **zero** advertising frameworks or tracking identifiers.

### 2.4. Local Preference Storage
User preferences (such as language selection, audio mute status, telemetry refresh interval, and custom user-defined ping targets) are stored strictly locally on your machine at `%LOCALAPPDATA%\ALLAHVERDCAN_THARP\tharp_settings.json`. This file is never synchronized to external cloud servers.

### 2.5. Compliance, GDPR/CCPA & Contact
Because THARP collects no personal information, there is no personal data held on our servers to access, rectify, or erase. For any inquiries, feature requests, or technical support, please contact:
- **Publisher:** ALLAHVERDİ CAN (`CN=80F86ABB-4ABB-4524-A032-0CE77FF05712`)
- **Email:** oguzyanardag@gmail.com