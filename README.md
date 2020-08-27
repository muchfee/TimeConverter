# TimeConverter
Diupload untuk memenuhi syarat ujian Modul 1
seconds=int(input("Masukkan detik: ")) #buat dulu variable seconds dengan input untuk memasukan angka
def timeConverter(seconds): #buat function dengan nama timeconverter
    hour = seconds // 3600 #Rumus menghitung jam
    seconds %= 3600  #Agar range tetap di 00-59
    minutes = seconds //60 #Rumus menhitung menit
    seconds %=60 #rumus menhitung detik agar range tetap di 00-59

    return "%02d:%02d:%02d" % (hour, minutes, seconds) #ini formatting string agar menjadi ("HH:MM:SS")
if seconds > 359999: #jika dia lebih dari 35999 maka akan menjadi invalid
    print("Invalid Input")
else: #jika tidak makan akan lanjut
    print(timeConverter(seconds))
