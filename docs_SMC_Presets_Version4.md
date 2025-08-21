# Preset Layout Pengaturan – Smart Money Concepts

Preset Tersedia
- Custom (default): gunakan pengaturan manual Anda (semua fitur advanced OFF secara default).
- Conservative: filtrasi ketat, kualitas sinyal prioritas.
- Balanced: seimbang antara jumlah sinyal dan kualitas.
- Aggressive: lebih longgar untuk menangkap lebih banyak peluang.
- Scalper: fokus eksekusi cepat LTF, filter minimal.
- Swing Trading (baru): kurasi POI kuat di anchor TF; konfirmasi di LTF.
- Ultra-Conservative (baru): filtrasi paling ketat untuk seleksi sinyal berkualitas tinggi.

Catatan Teknis
- Preset memengaruhi “effective settings” internal (eff*), tidak memaksa perubahan nilai input manual. Anda boleh override manual kapan saja.
- QS Label akan menambahkan emoji ⭐ saat preset “Swing Trading” atau “Ultra-Conservative” aktif untuk memudahkan pembacaan cepat.

Mapping Fitur Inti (ringkas)
- Conservative
  - Sweep: ON, PD: ON, FVG Confluence: ON (≤0.4 ATR)
  - Displacement BOS/CHoCH: ON (≥1.2 ATR, body/wick ≥0.5)
  - Confirmation Zones: ON, QS Label: ON
  - Partial Mitigation: 0.50, OTE: ON, Trailing: ON
  - Keep Mitigated: OFF, Show Invalidated: OFF
- Balanced
  - Sweep: ON, PD: ON, FVG Confluence: ON (≤0.5 ATR)
  - Displacement: ON (≥1.0 ATR, body/wick ≥0.5)
  - Confirmation: ON, QS: ON, Partial: 0.40, OTE: ON, Trailing: ON
  - Keep Mitigated: OFF, Show Invalidated: OFF
- Aggressive
  - Sweep: OFF, PD: OFF, Confluence: OFF (opsional ≤0.7 ATR)
  - Displacement: ON (≥0.8 ATR, body/wick ≥0.4)
  - Confirmation: ON, QS: ON, Partial: 0.30, OTE: ON, Trailing: ON
  - Keep Mitigated: OFF, Show Invalidated: OFF
- Scalper
  - Sweep: OFF, PD: OFF, Confluence: OFF
  - Displacement: OFF (konfirmasi internal di LTF)
  - Confirmation: OFF (opsional ON), QS: OFF, Partial: 0.30, OTE: OFF, Trailing: ON
  - Keep Mitigated: OFF, Show Invalidated: OFF
- Swing Trading (baru)
  - Sweep: ON, PD: ON, Confluence: ON (≤0.5 ATR)
  - Displacement: ON (≥1.1 ATR, body/wick ≥0.5)
  - Confirmation: ON, QS: ON, Partial: 0.50, OTE: ON, Trailing: ON
  - Keep Mitigated: OFF, Show Invalidated: OFF
- Ultra-Conservative (baru)
  - Sweep: ON, PD: ON, Confluence: ON (≤0.35 ATR)
  - Displacement: ON (≥1.5 ATR, body/wick ≥0.6)
  - Confirmation: ON, QS: ON (with ⭐), Partial: 0.60, OTE: ON, Trailing: ON
  - Keep Mitigated: OFF, Show Invalidated: OFF

Cara Pakai
1) Pilih preset di Settings indikator → “Preset”.
2) Opsional: tweak manual toggle untuk fine-tuning.
3) Simpan sebagai Template TradingView:
   - Atur preset/tweak → tombol tiga titik di dialog Settings → “Save as default”
   - Atau simpan Chart Layout dengan beberapa instance indikator (misal Conservative + Aggressive).

Tips Per Market
- FX/Crypto volatil tinggi: Balanced → Aggressive; jika banyak fakeouts, naikkan displacement (1.2–1.5 ATR).
- Indeks/large-cap: Conservative → Balanced; pertahankan PD & confluence ON.
- Swing multi-sesi: Swing Trading; manfaatkan Confirmation Zones + QS ≥ 3.
- Saring ekstra ketat saat kondisi choppy: Ultra-Conservative.