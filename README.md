# tim-anonymous-UI-frontend-smarthealth

**Tim Anonymous — Universitas Mikroskil**  
Laurencio Luckson (241110805) · Ervian Mentari · Shawn Michael · Jonathan Felix Fubrianto

---

## Stack
- **Framework**: React 18 + Vite
- **Styling**: Tailwind CSS
- **Routing**: React Router DOM v6
- **HTTP Client**: Axios
- **Notifikasi**: React Hot Toast

---

## Menjalankan Lokal

```bash
npm install
npm run dev
# → http://localhost:3000
```

Pastikan backend sudah berjalan di `http://localhost:5000`.

---

## Environment Variable

Buat file `.env` di root folder frontend:

```env
VITE_API_URL=https://smarthealth-backend.onrender.com
```

Untuk development kosongkan saja — sudah ada proxy Vite ke `localhost:5000`.

---

## Build Production

```bash
npm run build
# Output: folder dist/
```

---

## Struktur

frontend/
├── index.html
├── vite.config.js
├── tailwind.config.js
└── src/
    ├── App.jsx
    ├── main.jsx
    ├── index.css
    └── components/
        ├── Login.jsx
        ├── Register.jsx
        ├── Navbar.jsx
        ├── Home.jsx
        ├── Dashboard.jsx
        ├── StaffDashboard.jsx
        ├── Doctors.jsx
        ├── DoctorDetail.jsx
        ├── DoctorSchedule.jsx
        ├── Appointments.jsx
        ├── AppointmentHistory.jsx
        ├── HealthRecords.jsx
        ├── Services.jsx
        ├── Contact.jsx
        └── Footer.jsx

---

## Deploy ke render

1. Push repo ini ke GitHub
2. Buka [vercel.com](https://render.com) → **New Project** → Import repo
3. Setting:

| Field | Value |
|-------|-------|
| Build Command | `npm run build` |
| Output Directory | `dist` |

4. Tambah Environment Variable:

| Key | Value |
|-----|-------|
| `VITE_API_URL` | `https://smarthealth-backend.onrender.com` |

5. Klik **Deploy**

---
