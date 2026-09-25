## 🚀 AI Mentor — Initial Setup

Please follow these steps **in order**. Do not modify the application code yet.

### 1. Neon DB Setup

1. Go to Neon DB and create a new project.
2. **Project name:** `AI Mentor`
3. **Region:** `Singapore`
4. After creating the project, copy the **Database Connection String / Connection Snippet**.

Keep this connection string safe. **Do not commit it to GitHub.**

---

### 2. Create `.env` Files

There are `.env.example` files inside:

```text
backend/.env.example
frontend/.env.example
ai_service/.env.example
```

Create a copy of each `.env.example` file and rename the copies to:

```text
backend/.env
frontend/.env
ai_service/.env
```

So your structure should look like:

```text
AI-Mentor/
│
├── backend/
│   ├── .env.example
│   └── .env
│
├── frontend/
│   ├── .env.example
│   └── .env
│
└── ai_service/
    ├── .env.example
    └── .env
```

### 3. Configure Backend `.env`

Open:

```text
backend/.env
```

Find the database variable provided in `.env.example`, for example:

```env
DATABASE_URL=
```

Paste the **Neon DB connection string** after `=`:

```env
DATABASE_URL="your-neon-connection-string"
```

⚠️ **Important:** Do not delete or change the other variables in `.env` unless instructed.

---

### 4. Backend Setup

Open a terminal in the project root:

```bash
cd backend
npm install
```

---

### 5. Frontend Setup

Open another terminal:

```bash
cd frontend
npm install
```

---

### 6. AI Service Setup

Open another terminal:

```bash
cd ai_service
python -m venv venv
```

For **Windows PowerShell**:

```powershell
.\venv\Scripts\Activate.ps1
```

Then install the Python dependencies:

```bash
pip install -r requirements.txt
```

---

### ✅ Final Checklist

Before moving to the next task, make sure you have:

* [ ] Created the **AI Mentor** Neon DB project
* [ ] Selected **Singapore** region
* [ ] Copy env.example to  `backend/.env`
* [ ] Copy env.example to  `frontend/.env`
* [ ] Copy env.example to  `ai_service/backend/.env`
* [ ] Added the Neon DB connection string to `backend/.env`
* [ ] Run `npm install` inside `backend`
* [ ] Run `npm install` inside `frontend`
* [ ] Created and activated the Python virtual environment
* [ ] Installed `requirements.txt`

### ⚠️ Important

**Do NOT push `.env` files to GitHub.**
Only `.env.example` files should be committed.

If you face any error during setup, **send the error screenshot/message to Your Captain before changing anything manually.**
