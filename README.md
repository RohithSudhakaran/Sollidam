# 🌐 Sollidam (சொல்லிடம்) – Tamil Nadu's 3-Word Geocoding System

> 🧭 A modern location encoding system that converts GPS coordinates into simple, memorable 3-word addresses – tailored for Tamil Nadu.


---

## 🚀 Project Vision

**Sollidam** (சொல்லிடம்) is an open-source alternative to What3Words — made for Tamil Nadu.

❌ Problems with traditional Indian addresses:
- “2nd street near Murugan temple” — ambiguous and non-machine-readable
- Many areas lack house numbers
- Difficult for voice assistants and low-literacy users

✅ Sollidam’s Solution:
- Converts `GPS ↔ 3-word address`
- Tamil Nadu-specific
- Works without internet (coming soon)
- **Open-source** and free forever

---

## ✨ Key Features

- 🔁 **Bi-directional encoding**: GPS ⇄ 3-word code
- 🗺️ Interactive Leaflet-based grid map
- ⚡ Serverless API with REST support
- ✅ Tamil Nadu-specific logic
- 📡 Telegram Bot integration (Coming Soon)
- 🔓 Fully open-source

---

## 🧰 Tech Stack

| Layer        | Tech Used                                 |
| ------------ | ------------------------------------------ |
| Frontend     | React 18, TypeScript, React Router v6      |
| UI & Icons   | CSS3, Lucide React                         |
| Maps         | Leaflet.js                                 |
| API (Serverless) | TypeScript (Node.js), Vercel Functions  |

---

## 🌍 Live Links

🔗 **Main Application**:  
[`https://sollidam20.vercel.app`](https://sollidam20.vercel.app)

🔗 **API Base URL**:  
[`https://api-sollidam.vercel.app`](https://api-sollidam.vercel.app)


---

## 📡 REST API Usage

### 🔁 3-word ➝ Coordinates

```http
GET /api/lookup?words=word1.word2.word3
```

**Example:**
```http
GET https://api-sollidam.vercel.app/api/lookup?words=blue.sky.cloud
```

**Response:**
```json
{
  "lat": 8.795380650062402,
  "long": 77.53822544897345
}
```

---

### 🔁 Coordinates ➝ 3-word

```http
GET /api/lookup?location=latitude,longitude
```

**Example:**
```http
GET https://api-sollidam.vercel.app/api/lookup?location=11.0168,76.9558
```

**Response:**
```json
{
  "words": "moon.visitor.point"
}
```

---

## 🤖 Telegram Bot (Coming Soon)

Effortless location sharing:

- 🧭 Share location → Receive 3-word code + map link
- 📥 Send 3-word code → Get coordinates and location preview
- 🔗 Works without needing GPS apps

---

## 🛠️ Local Development

```bash
# Clone repository
git clone https://github.com/subhashraveendran/sollidam
cd sollidam

# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build
```

---

## 🧪 Testing

```bash
npm test               # Run unit tests
npm run accuracy-test  # Test grid accuracy
npm run stress-test    # Performance under heavy load
```

---


## 📜 License

Licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

Made with ❤️ in Tamil Nadu for **Hero’s on Wheels**  
#NenjeEzhu ✊
