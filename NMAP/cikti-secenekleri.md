## Çıktı Seçenekleri

### -oN → Normal Metin

```bash
nmap -oN tarama_sonucu.txt 192.168.1.1
```

### -oX → XML Formatında

```bash
nmap -oX tarama_sonucu.xml 192.168.1.1
```

### -oG → Grep İçin uygun formatta çıktı kaydetme

```bash
nmap -oG tarama_sonucu.grep 192.168.1.1
```

### -v (-vv -vvv) → Ayrıntılı (verbose) çıktı 

```bash
nmap -v 192.168.1.1
nmap -vv 192.168.1.1
nmap -vvv 192.168.1.1
```

### -d  → Hata ayıklama modu (debug)

```bash
nmap -d  192.168.1.1
```
