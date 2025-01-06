### -p <port> → belirli bir portu tarar 

- -p 80 → sadece 80 portunu tarar

```bash
nmap -p 80 192.168.1.1
```

- -p 22,80,443 → 22,80,443 portlarını tarar

```bash
nmap -p 22,80,443 192.168.1.1
```

- -p 1-65535  → 1 ile 65535 arasında olan bütün portları tarar

```bash
nmap -p 1-65535 192.168.1.1
```

### —top-ports <sayı> → En yaygın portları tarar

- —top-port 100 → en yaygın 100 portu tarar

```bash
nmap --top-port 100 192.168.1.1
```

### -p-   → Bütün portları tarar

```bash
nmap -p- 192.168.1.1
```

### —rondomoze-hosts → Hedeflerin tarama sırasını rastgeleleştirme  

```bash
nmap --rondomize-hosts 192.168.1.1
```
