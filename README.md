# prak-4
def ganti_vokal(teks):
    vokal = 'aiueoAIUEO'
    teks_baru = ''
    for huruf in teks:
        if huruf in vokal:
            teks_baru += 'i'
        else:
            teks_baru += huruf
    return teks_baru

def main():
    print("Masukkan teks lirik (3 kalimat):")
    lirik = input()
    kalimat = lirik.split('. ')
    lirik_baru = ''
    for kal in kalimat:
        lirik_baru += ganti_vokal(kal) + '. '
    print("Hasil:")
    print(lirik_baru)

if __name__ == "__main__":
    main()

