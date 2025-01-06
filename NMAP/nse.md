# NMAP SCRİPTİNG ENGİNE (NSE)

## SCRİPT Kategorileri

1. **auth** : Kimlik doğrulama 
2. **broadcast** : Ağdaki tüm cihazlarla iletişim kurar
3. **brute :** Bruteforce saldırıları
4. **discovery** : Bilgi Toplama
5. **exploit** : Zafiyet istismarları 
6. **intrusive** : Potansiyel olarak dikkat çekici işlemler 
7. **malware**: Zararlı yazılım analizi
8. **safe :** Hedef üzerinde zararsız taramalar

Tam listeye erişmek için 

```bash
ls /usr/share/nmap/scripts/
```

## —script Seçenekleri

—script=<script_ismi> → Belirli bir scripti çalıştırmak için kullanılır

Örnek

```bash
 nmap —script=http-title 192.168.1.1 
```

—script=<kategori> → Belirli kategoride ait scriptleri çalıştırır

Örnek

```bash
 nmap —script=vuln 192.168.1.1
```

## Popüler NSE Scriptleri

### Zaafiyet

—script=vuln → hedefte bilinen zaafiyetleri kontrol eder

Örnek

```bash
 nmap —script=vuln 192.168.1.1
```

### Web Uygulamaları

http-tittle → Hedef web sistesinin başlığını alır 

Örnek

```bash
nmap —script=http-tittle -p 80,443 ornek.com
```

http-enum → Web uygulamasındaki yaygın dosya ve dizinleri listeler

Örnek

```bash
 nmap —script=http-enum 192.168.1.1
```

### Şifre Kontrolü

ftp-anon → FTP anonim giriş kontrolü 

Örnek

```bash
 nmap —script=ftp-anon -p 21 192.168.1.1
```

ssh-brute → SSH kaba kuvvet saldırı

Örnek

```bash
 nmap —script=ssh-brute -p 22 192.168.1.1
```

### Zararlı Dosyalar ve İstismar

smb-vuln-ms17-010 → EternalBlue zafiyetine kontrol eder

Örnek

```bash
nmap —script=smb-vuln-ms17-010 -p 445 192.168.1.1
```

## Genel Bilgi Toplama

dns-brute → DNS Alan adlarına brute force yapar 

Örnek

```bash
 nmap —script=dns-brute example.com
```

snmp-info → SNMP üzerinden bilgi toplar 

Örnek

```bash
 nmap —script=snmp-info -p 161 192.168.1.1
```
