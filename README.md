<div align="center">

# 🔐 Online Hash Crackers & Hash Lookup Tools

**Koleksi online hash lookup, hash cracking services, reverse hash databases, MD5/SHA lookup tools, dan password recovery references untuk CTF, lab, defensive security, SOC enrichment, dan authorized password audit.**

![Focus](https://img.shields.io/badge/focus-hash%20lookup%20%7C%20hash%20cracking%20%7C%20password%20audit-7F77DD?style=flat-square)
![Usage](https://img.shields.io/badge/usage-ethical%20only%20%7C%20authorized-D85A30?style=flat-square)
![Category](https://img.shields.io/badge/category-crypto%20%7C%20password%20security%20%7C%20DFIR-1D9E75?style=flat-square)

</div>

---

> Repository ini berisi layanan online untuk **hash lookup**, **reverse hash search**, dan **authorized password recovery**.  
> Gunakan hanya untuk hash milik sendiri, CTF/lab, audit internal berizin, SOC/DFIR enrichment, atau proses recovery yang sah.

---

## 📑 Daftar Isi

- [🎯 Purpose](#-purpose)
- [🔎 Online Hash Lookup & Reverse Hash Databases](#-online-hash-lookup--reverse-hash-databases)
- [🧪 MD5-Focused Lookup & Cracking Resources](#-md5-focused-lookup--cracking-resources)
- [🧰 Online Hash Cracking Services](#-online-hash-cracking-services)
- [🛡️ Defensive Password Audit & Exposure Checking](#️-defensive-password-audit--exposure-checking)
- [⚠️ Parked / Suspicious / Unverified Links](#️-parked--suspicious--unverified-links)
- [🧭 Safe Workflow](#-safe-workflow)
- [🔐 Safety Notes](#-safety-notes)
- [⚖️ Disclaimer](#️-disclaimer)

---

## 🎯 Purpose

Online hash lookup dan hash cracking tools berguna untuk:

- CTF dan lab password cracking
- Recover password milik sendiri
- Mengecek apakah hash sudah ada di database publik
- SOC/DFIR enrichment terhadap artefak hash
- Validasi password hygiene dalam audit internal
- Membantu edukasi tentang weak hashing dan password reuse
- Menguji apakah hash lemah seperti MD5/SHA1 mudah ditemukan

---

## 🔎 Online Hash Lookup & Reverse Hash Databases

| Tool | Link | Fungsi |
|---|---|---|
| CrackStation | https://crackstation.net/ | Large hash lookup database untuk password hash umum seperti LM, NTLM, MD5, SHA1, SHA256, dan lainnya. |
| SANS ISC Reverse Hash Lookup | https://isc.sans.edu/tools/reversehash.html | Reverse hash lookup dari SANS Internet Storm Center untuk membantu analisis hash secara defensif. |
| MD5Decryption | https://md5decryption.com/ | Reverse lookup untuk MD5 dan beberapa hash umum dari database publik. |
| Hashes.com | https://hashes.com/en/decrypt/hash | Online hash lookup/decrypt database untuk beberapa tipe hash umum. |
| HashKiller | https://hashkiller.io/ | Hash cracking dan lookup community/resource untuk password audit dan lab. |
| md5hashing.net | https://md5hashing.net/hash | Online hash generator dan lookup untuk berbagai algoritma hash. |

---

## 🧪 MD5-Focused Lookup & Cracking Resources

| Tool / Resource | Link | Fungsi |
|---|---|---|
| CMD5 | https://www.cmd5.org/ | Online hash cracking/lookup service yang populer untuk MD5 dan beberapa hash lain. |
| Tydal MD5 Crack Article | https://www.tydal.nu/article/md5-crack/ | Artikel/resource lama tentang MD5 cracking; berguna sebagai referensi historis/edukasi. |
| MD5Decryption | https://md5decryption.com/ | Lookup MD5 dari database publik. |
| CrackStation | https://crackstation.net/ | Lookup hash umum, termasuk MD5. |
| OnlineHashCrack | https://www.onlinehashcrack.com/ | Online password/hash recovery service untuk berbagai format hash/file tertentu. |

---

## 🧰 Online Hash Cracking Services

| Tool | Link | Fungsi |
|---|---|---|
| OnlineHashCrack | https://www.onlinehashcrack.com/ | Online hash/password recovery service untuk audit legal dan recovery milik sendiri. |
| CrackStation | https://crackstation.net/ | Fast hash lookup database untuk hash umum. |
| CMD5 | https://www.cmd5.org/ | Online hash lookup/cracking service. |
| HashKiller | https://hashkiller.io/ | Community-based hash lookup/cracking resource. |
| GPUHash.me | https://gpuhash.me/ | Online GPU-assisted hash cracking service; gunakan hanya untuk hash milik sendiri atau audit berizin. |

---

## 🛡️ Defensive Password Audit & Exposure Checking

| Resource | Link | Fungsi |
|---|---|---|
| Have I Been Pwned - Pwned Passwords | https://haveibeenpwned.com/Passwords | Mengecek apakah password/hash sudah muncul di breach corpus dengan model k-anonymity. |
| Have I Been Pwned API | https://haveibeenpwned.com/API/v3 | API untuk breach/password exposure checking secara defensif. |
| SecLists Passwords | https://github.com/danielmiessler/SecLists/tree/master/Passwords | Wordlist untuk lab, audit internal, dan password policy testing legal. |
| Weakpass | https://weakpass.com/ | Wordlist dan password lists untuk audit internal/lab. |
| Openwall Wordlists | https://www.openwall.com/wordlists/ | Wordlists untuk password security testing dan audit legal. |

---

## ⚠️ Parked / Suspicious / Unverified Links

> Link di bagian ini **tidak direkomendasikan sebagai tool utama**. Simpan sebagai catatan agar tidak tercampur dengan resource yang lebih terpercaya.

| Resource | Link | Catatan |
|---|---|---|
| md5crack.com via GoDaddy Domain Search | https://www.godaddy.com/en-ph/domainsearch/find?isc=AFT_UNA&tmskey=dpp_dbs&domainToCheck=md5crack.com | Ini terlihat seperti halaman pencarian/penjualan domain, bukan layanan hash cracking aktif. |
| albaniazx38.60ma.net | http://albaniazx38.60ma.net/ | Link tidak jelas/suspicious/unverified. Jangan jadikan rekomendasi utama tanpa audit manual. |

---

## 🧭 Safe Workflow

```text
1. Identify hash type
   ↓
2. Check whether the hash is non-sensitive and allowed to test
   ↓
3. Try lookup-only services first
   - CrackStation
   - SANS Reverse Hash
   - MD5Decryption
   ↓
4. Use online cracking service only for authorized hash
   ↓
5. Document result and confidence
   ↓
6. Recommend stronger hashing if weak hash is found
```

### Example Defensive Use Cases

```text
CTF / lab:
Identify hash → CrackStation → MD5Decryption → OnlineHashCrack

SOC enrichment:
Hash from log/artifact → SANS Reverse Hash → CrackStation → HIBP Pwned Passwords

Internal audit:
Hash sample with permission → lookup/check exposure → document weak password risk
```

---

## 🔐 Safety Notes

Jangan upload atau cek hash secara sembarangan. Hash tetap bisa sensitif karena dapat merepresentasikan password asli, token, credential, atau data internal.

Sebelum memakai online service, pastikan:

- Hash milik kamu sendiri atau audit internal berizin
- Bukan data customer
- Bukan credential produksi
- Bukan password/token/API key internal
- Tidak melanggar scope bug bounty
- Tidak berasal dari breach, dump, atau akses tidak sah

Untuk data sensitif, gunakan lab lokal/offline tools dan jangan upload ke layanan publik.

---

## ⚖️ Disclaimer

Gunakan resource ini hanya untuk:

- CTF
- Lab pribadi
- Password recovery milik sendiri
- Internal password audit berizin
- SOC/DFIR enrichment
- Security education
- Defensive security research

Jangan gunakan layanan ini untuk cracking hash hasil pencurian, credential stuffing, mengambil alih akun, memproses data breach tanpa izin, atau aktivitas yang melanggar hukum.
