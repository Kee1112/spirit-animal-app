# 🐾 Spirit Animal Finder (Full‑Stack App)

A beginner‑friendly **full‑stack web app** built to understand how a frontend communicates with a backend.

Users enter their name, the backend counts the number of vowels, and returns a fun **spirit animal** 🔥🐉🐎🦄. The frontend displays the result along with animated illustrations.

This project is intentionally simple and clean, focusing on **core concepts** rather than complexity.

---

## ✨ Features

* 🌐 Frontend built with **HTML, CSS, JavaScript**
* ⚡ Backend built with **FastAPI (Python)**
* 🔁 Real HTTP communication using `fetch()`
* 🧠 Business logic handled in the backend
* 🎨 Animated illustrations (Storyset / SVG / GIF)
* ☁️ Deployed using **Netlify (frontend)** and **Render (backend)**

---

## 🗂️ Project Structure (Showcase Repo)

```
spirit-animal-app/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── README.md
│
├── frontend/
│   ├── index.html
│   └── static/
│       └── style.css
│
└── README.md
```

> ⚠️ Note: This is a **showcase repository**. Frontend and backend are deployed from **separate repos**.

---

## 🚀 Live Demo

* **Frontend (Netlify):** https://<your-netlify-url>
* **Backend (Render):** https://<your-render-url>
* **API Docs:** https://<your-render-url>/docs

---

## 🧠 How It Works

1. User enters their name in the frontend
2. Frontend sends a `POST` request to the backend
3. Backend:

   * counts vowels in the name
   * maps vowel count → spirit animal
4. Backend returns JSON response
5. Frontend updates the UI dynamically

Example response:

```json
{
  "name": "Keerthana",
  "vowel_count": 4,
  "spirit_animal": "🐺 Wolf"
}
```

---

## 🧪 Run Locally

### 1️⃣ Backend

```bash
cd backend
python -m venv venv
venv\Scripts\activate   # Windows
pip install -r requirements.txt
uvicorn main:app --reload
```

Backend runs at:

```
http://127.0.0.1:8000
```

---

### 2️⃣ Frontend

Update API URL in `index.html`:

```js
fetch("http://127.0.0.1:8000/spirit_animal")
```

Then either:

* open `index.html` directly in the browser, **or**
* run a local server:

```bash
cd frontend
python -m http.server 5500
```

Open:

```
http://localhost:5500
```

---

## ☁️ Deployment

### Backend

* Deployed on **Render**
* Auto‑redeploys on every GitHub push

### Frontend

* Deployed on **Netlify**
* Static site hosting
* Auto‑redeploys on GitHub push

Frontend and backend are **decoupled**, following real‑world architecture.

---

## 🎯 Why This Project

This project was built to:

* understand **frontend ↔ backend communication**
* learn **API design basics**
* practice **deployment workflows**
* gain confidence in full‑stack development

It prioritizes **clarity and fundamentals** over frameworks and abstractions.

---

## 🔮 Future Improvements

* Add loading states & error handling
* Environment‑based API URLs
* Docker setup for one‑command run
* More animations & themes
* Database support

---

## 🧑‍💻 Author

Built with curiosity and the urge to understand how apps actually work .
I must add this project helped me clear all my doubts and actually gave me a crystal clear 
understanding of how APIs work and how JS communicates with the backend.

If you’re learning full‑stack development — feel free to fork, clone, and experiment!
