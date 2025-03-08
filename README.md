Güvenli Veri İletim Protokolü

Bu proje, İnsansız Hava Araçları (İHA) ve uydular arasında veri bütünlüğünü ve gizliliğini sağlamak için güvenli bir iletişim protokolü geliştirmeyi ve başlangıç seviyesinde simüle etmeyi amaçlamaktadır. AES şifreleme ile birlikte CRC-64 hata tespit algoritmalarından yararlanarak, veri iletimi için özel bir protokol oluşturuyoruz. Bu proje, iletişim sürecini simüle etmek ve güvenli hale getirmek için ARM ve AVR mikrodenetleyici platformları olan Arduino Uno ve Raspberry Pi 2'nin bir kombinasyonunu kullanır.

Donanım Bileşenleri

Linux Server: İletişimi başlatmak ve son veri alımı

Arduino Uno (AVR mimarisi): CRC-32 kullanarak veri bütünlüğünü sağlama ve başlangıç veri işleme

Raspberry Pi 2 (ARM mimarisi): CRC-64 kullanarak daha fazla veri doğrulama ve veri işleme

SLA 3D Yazıcı ve Bakır Plakalar: Prototip devre kartlarını oluşturmak için

USB Kabloları: Server, Arduino Uno ve Raspberry Pi 2 bağlantısı

Jumper Kabloları: Arduino Uno ve Raspberry Pi 2 arasındaki UART iletişimi

Yazılım Bileşenleri

Arduino IDE: Arduino Uno'ya kod geliştirmek ve yüklemek

Rust: Raspberry Pi 2 üzerinde şifreleme ve veri işleme kodu yazmak

C++ (satır içi montaj ile): Arduino Uno üzerinde düşük seviyeli UART iletişimi ve veri işleme uygulamak

WiringPi: Raspberry Pi 2 üzerinde GPIO ve UART kullanımı

Projenin İkinci Etabı

SLE (Synchronous Link Encryption) Protokolü SLE protokolü, güvenli veri iletimi sağlamak için kullanılan bir şifreleme protokolüdür. SLE, veri paketlerinin şifrelenmiş ve zaman uyumlu bir şekilde iletilmesini sağlar. İkinci etapta SLE protokolünü kullanarak veri iletim güvenliğini bir adım daha ileri taşıyacağız.

SLE Protokolünün Özellikleri

Zaman Uyumu (Synchronous Timing): Verilerin belirli zaman aralıklarında iletilmesini sağlar

Güvenli Şifreleme: AES gibi güçlü şifreleme algoritmaları kullanarak verinin gizliliğini korur

Veri Bütünlüğü: Hata tespit mekanizmaları (örneğin, CRC) ile verinin bütünlüğünü sağlar

RISC-V Mimarisinde Assembly Kod Betikleri RISC-V, açık kaynaklı ve modüler bir komut seti mimarisidir (ISA). Projenin ikinci etabında, RISC-V mimarisi üzerine inşa edilen mikroişlemciler kullanarak veri işleme ve iletişim protokollerini geliştireceğiz. Aşağıda, RISC-V assembly dilinde bazı temel komut örneklerini bulabilirsiniz.
