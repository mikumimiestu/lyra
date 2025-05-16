# 🌸 Lyra API - AI Endpoint by Tech Nova Group

![Powered by Lyra 1.0 Base](https://img.shields.io/badge/Model-Lyra%201.0%20Base-87cefa?style=flat-square&logo=sparkles&logoColor=white)
![Powered by Lyra 1.0 Prime](https://img.shields.io/badge/Model-Lyra%201.0%20Prime-b57edc?style=flat-square&logo=sparkles&logoColor=white)
![Powered by Lyra 1.5 Luma](https://img.shields.io/badge/Model-Lyra%201.5%20Luma-ffb6c1?style=flat-square&logo=sparkles&logoColor=white)

Lyra API adalah layanan AI endpoint yang menggunakan model Gemini Flash 2.5 sebagai backend, namun dibungkus dan dikembangkan ulang melalui model internal:

| Model Name        | Parameters | Deskripsi Singkat                                   |
|-------------------|------------|-----------------------------------------------------|
| **Lyra 1.0 Base** | 1B         | Model ringan dan cepat untuk keperluan general NLP. |
| **Lyra 1.0 Prime**| 0.5B       | Versi super ringan, cocok untuk mobile & latency.   |
| **Lyra 1.5 Luma** | 4B         | Model powerful dengan pemahaman lebih mendalam.     |

---

## 🔌 Endpoint Publik

Semua request dilakukan via `POST` ke endpoint berikut:

POST https://lyra.technovagroupinc.com/api/lyra

### 🧾 Request Body Example

```json
{
  "prompt": "Halo Lyra, apa itu machine learning?",
  "model": "lyra-1.0-base"
}
```

| Parameter                | Tipe                          | Keterangan                                |
| -------------------- | --------------------------------- | ----------------------------------------- |
| ```prompt```         | string                            | Pertanyaan atau instruksi pengguna.       |
| ```model```          | string                            | Pilih model (lyra-1.0-base, lyra-1.0-prime, lyra-1.5-luma) — default: lyra-1.5-base    |

### 🧾 Headers

```http
Content-Type: application/json
x-api-key: YOUR_API_KEY
```

### 🔐 Keamanan

- Gunakan x-api-key di header untuk akses endpoint.
- Key bisa didapatkan melalui pendaftaran ke tim Tech Nova Group.
- Rate limit per key akan diberlakukan untuk mencegah penyalahgunaan.

### 🧠 Tentang Lyra

Lyra adalah AI assistant buatan Technova Group yang dirancang untuk menjadi rekan digital cerdas, bisa digunakan untuk menjawab pertanyaan, membuat ringkasan, membantu pemrograman, hingga eksplorasi ide.

> 🌟 Powered by Gemini, OpenAI, Llama, Qwen, DeepSeek and Anthropic under the hood, with Lyra's own personality & optimization layer.
