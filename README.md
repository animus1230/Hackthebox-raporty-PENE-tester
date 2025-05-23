# Pentesting Portfolio

**Kevin **: [Kevin ]

**Wiek**: 17 lat

**Kierunek**: Pene Tester w Cyberbezpieczeństwie

**O mnie**
Jestem młodym entuzjastą bezpieczeństwa IT, który pasjonuje się znajdowaniem i eksploatacją podatności systemów. Mimo ograniczonego czasu, aktywnie rozwijam swoje umiejętności poprzez praktyczne wyzwania na platformie HackTheBox. Każdego dnia uczę się czegoś nowego i doskonalę techniki pentestingu, aby w przyszłości stać się cenionym specjalistą w branży.

---

## 🎯 Cele zawodowe
- Stać się wszechstronnym pentesterem z umiejętnością przeprowadzania testów od wewnątrz i z zewnątrz sieci.
- Opanować narzędzia i techniki takie jak Nmap, Metasploit, Burp Suite, skrypty Python/Bash oraz exploit development.
- Zdobyć certyfikat OSCP lub równoważny, aby potwierdzić swoje kompetencje.

---

## 🛠️ Umiejętności techniczne
- **Skanowanie i rozpoznanie**: Nmap, Masscan, RustScan
- **Eksploatacja**: Metasploit Framework, custom NSE scripts, RCE
- **Automatyzacja**: Skrypty Bash i Python (Scapy, Paramiko)
- **Analiza ruchu sieciowego**: Wireshark, tcpdump
- **Privilege Escalation**: SUID/SGID binaries, misconfigurations
- **Systemy operacyjne**: Linux (Debian, Ubuntu), Windows
- **Kontrola wersji**: Git, GitHub

---

## 📂 Projekty i doświadczenie

### Virtual HackTheBox: **"Green"**
- **Krok 1 – Discovery**: Przeprowadziłem ping sweep oraz skan portów TCP (`nmap -sC -sV -p-`) w celu zidentyfikowania otwartych usług.
- **Krok 2 – Rozpoznanie**: Odkryłem, że port 22 (SSH) oraz port 80 (HTTP) były dostępne. Zanalizowałem nagłówki HTTP i odkryłem wątpliwe parametr w panelu administracyjnym.
- **Krok 3 – Eksploatacja**:
  - Stworzyłem **skrypt Python** wykorzystujący bibliotekę **Paramiko** do automatycznego brute-force’u SSH z listą 100 popularnych haseł.
  - Użyłem **Nmap NSE** do identyfikacji podatnych wersji serwera SSH oraz do automatyzacji zdalnego wykonania komend.
- **Krok 4 – Dostęp niskiego poziomu**: Uzyskałem dostęp do konta użytkownika `htbuser` i zebrałem pliki konfiguracyjne.
- **Krok 5 – Podniesienie uprawnień**:
  - Zidentyfikowałem **SUID binary** z nieprawidłowymi uprawnieniami.
  - Zaimplementowałem **custom Bash exploit**, który pozwolił uzyskać sesję roota.
- **Efekt**: Pełny dostęp do systemu operacyjnego jako **root**, potwierdzony zrzutem ekranu flagi `/root/root.txt`.

### Virtual HackTheBox: **"Cherry"**
- **Discovery**: Wykonałem ping sweep sieciowe i skan UDP (`nmap -sU`) aby wyszukać usługi DNS i SNMP.
- **Eksploatacja SNMP**:
  - Napisałem **skrypt Python** korzystający z **Scapy**, aby zautomatyzować odpytywanie SNMP.
  - Odkryłem domyślną społeczność `public` i wyciągnąłem wrażliwe informacje o użytkownikach.
- **Privilege Escalation**: Wykorzystałem błąd w konfiguracji plików cron, dodając zadanie, które dało mi root.

---

## 📈 Ciągły rozwój
- Regularnie uczestniczę w CTF-ach hacker 101 (Capture The Flag).
- Uczę się exploit development (buffer overflow, format string).
- Planuję certyfikację OSCP w ciągu najbliższych 15 miesięcy.

---

## 📬 Kontakt
- **Email**: bibip0662@gmail.com
- **GitHub**: https://github.com/animus1230


---

