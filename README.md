# Toshkent IEM — Unit 1 CCGT O'quv Treneri

> **AVTONOM O'QUV STENDI — real DCS/PLC ga ulanmagan.**
> Mitsubishi M701F + Honeywell Experion PKS / Yokogawa CENTUM VP uslubidagi
> HMI simulyatsiyasi. Real boshqaruv uchun ishlatilmaydi.

## Fayllar

| Fayl | Tavsif |
|---|---|
| `unit1-ccgt-trainer.html` | Asosiy trener (v2.x): Overview, GT, HRSG 3-bosimli, ST, Electrical 110 kV, Trend/Alarm. Bitta fayl, internet shart emas |
| `index.html` | Eski v1.0 maket (arxiv) |

## Ishga tushirish

`unit1-ccgt-trainer.html` ni brauzerda oching (ikki marta bosing).
Windows da o'rnatish kerak emas, fleshka bilan IEM kompyuteriga ko'chirish mumkin.

## Yurgizish tartibi (interlock bilan)

1. CEP → FWP → CW (suv + vakuum)
2. FV → GT START (3000 rpm)
3. 52H → GT SYNC (52G) → AVR AUTO → yuk 150–230 MW
4. HRSG bosim → MSV-HP → IP-ADM
5. ST ROLL (vakuum <−60 kPa shart) → SYNC → yuk 80–120 MW

## Instruktor ssenariylari

Fuel↓, Drum, Freq 49.4 Hz, VIB↑, Oil↓, Overspeed.
Reaksiya normasi 15 s — jurnal `.txt` saqlanadi, OK/XATO hisobi yuritiladi.

## Standart parametrlar

GT 2995–3005 rpm • Fuel 2.5–3.2 MPa • EXH 550–620 °C •
HP 10–12 MPa / 535 °C • IP 2.5–3.0 MPa • LP 0.5–0.7 MPa •
Drum ±50 mm (trip ±80) • ST 80–120 MW • Freq 50.00 Hz (<49.5 alarm) •
VIB >125 trip • BRG >110 trip • Oil <0.20 trip •
GEN 15.75 kV • GRID 110 kV • cosφ 0.85–0.90

## GitHub

Loyiha GitHub da saqlanadi. Tokenni hech kimga bermang,
faqat o'z kompyuteringizda `git push` paytida kiriting.
