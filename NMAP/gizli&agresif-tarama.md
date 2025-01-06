## Gizli ve Agresif Taramalar

### —spoof-mac → Sahte bir MAC adresi kullanma 

```bash
nmap -sS --spoof-mac 00:11:22:33:44:55 192.168.1.1
```

### -D → Decoy IP kullanmak izin gizleme 

```bash
nmap -sS -D 192.168.1.10,192.168.1.20,ME 192.168.1.1
```

### —badsum → Hatalı TCP/UDP checksumları ile test yapar 

```bash
nmap --badsum 192.168.1.1
```

### —source-port → Kaynak portunu belirlemek için kullanılır

```bash
nmap -sS --source-port 80 192.168.1.1
```

### -n → DNS çözümleyiciyi devre dışı bırakmak için kullanılır 

```bash
nmap -n -sP 192.168.1.0/24
```
