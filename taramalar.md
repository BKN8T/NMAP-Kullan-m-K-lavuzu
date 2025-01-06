# Tarama Türleri ve Parametreler

### -sS   →SYN Taraması

```bash
nmap -sS 192.168.1.1
```

### -sA   →ACK Taraması(Güvenlik duvarlarının yapılandırılmasını kontrol etmek için kullanılır)

```bash
nmap -sA 192.168.1.1
```

### -sN   →NULL Taraması(Herhangi bir TCP bayrağı olmadan tarama yapar)

```bash
nmap -sN 192.168.1.1
```

### -sT    →Tam bir TCP bağlantısı Kurar SYN taramasına izin verilmediğinde kullanılır

```bash
nmap -sT 192.168.1.1
```

### -sU   →UDP Taraması

```bash
nmap -sU 192.168.1.1
```

### -sV   →Servis ve Versiyon taraması için kullanılır

```bash
nmap -sV 192.168.1.1
```

### -sP   →Ping Taraması. Hedefin çevrimiçi olup olmadığını kontrol eder. Nmap’in yeni sürümlerinde -sn olarak değiştirilmiştir (yalnızca host keşfi yapar, port taramaz).

```bash
nmap -sP 192.168.1.1
nmap -sn 192.168.1.1
```

### -O    → İşletim sistemi tahmini yapar 

```bash
nmap -O 192.168.1.1
```

### —osscan-guess → Daha agresif işletim sistemi tahmini

```bash
nmap --osscan-guess 192.168.1.1
```

### —traceroute → Traceroute bilgisi ekler

```bash
nmap --traceroute 192.168.1.1
```

### -A    → Ayrıntılı tarama (OS tespiti, servis versiyon bilgisi ve traceroute dahil)

```bash
nmap -A 192.168.1.1
```

### -Pn  →Ping atmadan tarama yapar

```bash
nmap -Pn 192.168.1.1
```

### -PR  →ARP ping taraması

```bash
nmap -PR 192.168.1.1
```

### -6    →IPv6 adresi kullanarak tarama 

```bash
nmap -6 2001:db8:85a3::8a2e:370:7334
```

### —reason → Hedef hakkında daha fazla bilgi verir

```bash
nmap --reason 192.168.1.1
```

### -f → paketleri daha küçük parçalara bölerek güvenlik duvarlarını atlatma

```bash
nmap -sS -f 192.168.1.1
```
