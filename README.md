# effective-waffledef hitung_wafel(tepung, telur, susu):
    # Asumsi tiap wafel butuh 100g tepung, 1 telur, 200ml susu
    jumlah_dari_tepung = tepung // 100
    jumlah_dari_telur = telur // 1
    jumlah_dari_susu = susu // 200
    return int(min(jumlah_dari_tepung, jumlah_dari_telur, jumlah_dari_susu))

if __name__ == "__main__":
    try:
        tepung = float(input("Masukkan jumlah tepung (gram): "))
        telur = float(input("Masukkan jumlah telur (butir): "))
        susu = float(input("Masukkan jumlah susu (ml): "))
        hasil = hitung_wafel(tepung, telur, susu)
        print(f"Jumlah wafel maksimal yang bisa dibuat: {hasil}")
    except ValueError:
        print("Input tidak valid. Silakan masukkan angka.")
