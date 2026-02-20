# 🚀 Snippets REST API — Beautiful & Practical Docs

<p align="center">
  <b>Simple code snippets API</b> · Built for learning REST with Django REST Framework
</p>

<p align="center">
  <img alt="API" src="https://img.shields.io/badge/API-REST-6f42c1" />
  <img alt="Methods" src="https://img.shields.io/badge/Methods-GET%20POST%20PUT%20DELETE-0ea5e9" />
  <img alt="Auth" src="https://img.shields.io/badge/Auth-Basic-orange" />
  <img alt="Status" src="https://img.shields.io/badge/Hosted%20on-Render-46E3B7" />
</p>

---

## ⚠️ IMPORTANT WARNING / AVISU IMPORTANTE (Read First / Lee uluk)

### ENGLISH
If you are testing this API on Render free tier, the server can be "sleeping".
On the first request, you may need to wait **50 seconds to 1+ minute** for the server to wake up.

✅ Please be patient and try again if your first request is slow.

### TETUN
Se ita teste API ida-ne'e iha Render free tier, servidor bele iha kondisaun "sleeping".
Iha request dahuluk, ita presiza hein **50 segundu to'o liu 1 minutu** atu servidor fila fali.

✅ Favor paciencia no koko fila fali se request dahuluk la'o kleur.

---

## 📘 API Overview (English)

The **Snippets REST API** lets you:
- Get all snippets
- Get one snippet by ID
- Create a new snippet
- Update a snippet
- Delete a snippet

**Base URL**
```txt
https://juliao-martins-snippets.onrender.com
```

### 1) Get all snippets (GET)
```http
GET /snippets/
```

Postman URL:
```txt
https://juliao-martins-snippets.onrender.com/snippets/
```

### 2) Get a specific snippet (GET)
```http
GET /snippets/1/
```

Postman URL:
```txt
https://juliao-martins-snippets.onrender.com/snippets/1/
```

### 3) Create snippet (POST)
```bash
postman request POST 'https://juliao-martins-snippets.onrender.com/snippets/' \
  --header 'Content-Type: application/json' \
  --header 'Authorization: Basic anVsaWFvOmp1bGlhb0BkZXYxMjM=' \
  --body '{
    "code": "using System;\r\n\r\nnamespace HelloWorldApp\r\n{\r\n    class Program\r\n    {\r\n        static void Main(string[] args)\r\n        {\r\n            Console.WriteLine(\"Hello, World!\");\r\n            // Optional: Keep the console window open in some environments\r\n            // Console.ReadKey(); \r\n        }\r\n    }\r\n}"
}' \
  --auth-basic-username 'secret_username' \
  --auth-basic-password 'secret_password'
```

### 4) Update snippet (PUT)
```bash
postman request PUT 'https://juliao-martins-snippets.onrender.com/snippets/3/' \
  --header 'Content-Type: application/json' \
  --header 'Authorization: Basic anVsaWFvOmp1bGlhb0BkZXYxMjM=' \
  --body '{
    "code": "\\ My first program\r\n\rusing System;\r\n\r\nnamespace HelloWorldApp\r\n{\r\n    class Program\r\n    {\r\n        static void Main(string[] args)\r\n        {\r\n            Console.WriteLine(\"Hello, World!\");\r\n            // Optional: Keep the console window open in some environments\r\n            // Console.ReadKey(); \r\n        }\r\n    }\r\n}"
}' \
  --auth-basic-username 'secret_username' \
  --auth-basic-password 'secret_password'
```

### 5) Delete snippet (DELETE)
```bash
postman request DELETE 'https://juliao-martins-snippets.onrender.com/snippets/3/' \
  --header 'Content-Type: application/json' \
  --header 'Authorization: Basic anVsaWFvOmp1bGlhb0BkZXYxMjM=' \
  --body '{
    "code": "\\ My first program\r\n\rusing System;\r\n\r\nnamespace HelloWorldApp\r\n{\r\n    class Program\r\n    {\r\n        static void Main(string[] args)\r\n        {\r\n            Console.WriteLine(\"Hello, World!\");\r\n            // Optional: Keep the console window open in some environments\r\n            // Console.ReadKey(); \r\n        }\r\n    }\r\n}"
}' \
  --auth-basic-username 'secret_username' \
  --auth-basic-password 'secret_password'
```

---

## 📗 Esplicasaun API (Tetun)

**Snippets REST API** bele ajuda ita atu:
- Hetan lista snippets hotu-hotu
- Hetan snippet ida tuir ID
- Kria snippet foun
- Atualiza snippet ida
- Hamos snippet ida

**Base URL**
```txt
https://juliao-martins-snippets.onrender.com
```

### 1) Hetan snippets hotu (GET)
```http
GET /snippets/
```

### 2) Hetan snippet espesífiku (GET)
```http
GET /snippets/1/
```

### 3) Kria snippet (POST)
Uza request hanesan iha seksaun Ingles, ho autenticasaun Basic no JSON body.

### 4) Atualiza snippet (PUT)
Uza request hanesan iha seksaun Ingles, altera `code` tuir presiza.

### 5) Hamos snippet (DELETE)
Uza request hanesan iha seksaun Ingles atu hamos snippet tuir ID.

---

## 🧪 Quick Testing Tips
- First request might be slow (Render cold start).
- Use Postman and set `Content-Type: application/json`.
- For write operations (`POST`, `PUT`, `DELETE`), include Basic Auth.
- If timeout happens on first try, wait and retry once.

---

## ❤️ Thanks
If this API helps your learning journey, star the repository and share it with friends.
