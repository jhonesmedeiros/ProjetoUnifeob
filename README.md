Estrutura do projeto
brasa-brothers/
├─ backend/
│ ├─ package.json
│ ├─ src/
│ │ ├─ index.js
│ │ ├─ db.js
│ │ ├─ routes/
│ │ │ ├─ auth.js
│ │ │ ├─ products.js
│ │ │ └─ orders.js
│ │ └─ middleware/
│ │ └─ authMiddleware.js
│ └─ .env.example
├─ frontend/
│ ├─ package.json
│ ├─ index.html
│ └─ src/
│ ├─ main.jsx
│ ├─ App.jsx
│ ├─ pages/
│ │ ├─ Login.jsx
│ │ ├─ Register.jsx
│ │ ├─ Menu.jsx
│ │ ├─ Cart.jsx
│ │ └─ Checkout.jsx
│ ├─ components/
│ │ ├─ Header.jsx
│ │ └─ ProductCard.jsx
│ └─ services/
│ └─ api.js
1
├─ README.md
└─ .gitignore
