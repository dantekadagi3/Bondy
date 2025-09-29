
```markdown
#  Bond Analysis Platform

A beginner-friendly web platform for analyzing government bonds.  
Users can upload bond prospectuses (in PDF format), view simplified summaries, calculate investment returns, compare bonds side by side, and generate downloadable reports.

---

##  Features
- **PDF Upload & Parsing** → Extracts bond details (coupon rate, maturity, tax, etc.) automatically.  
- **Bond Summaries** → Presents key information in simple, newbie-friendly language.  
- **Investment Calculator** → Enter an amount and see semi-annual payouts, yearly earnings, and total maturity value.  
- **Bond Comparison Tool** → Compare multiple bonds and see which offers better returns vs shorter maturity.  
- **Reports** → Export results to **PDF or Excel** for offline use.  
- **User Portfolio (optional)** → Save bonds and track upcoming coupon payments.  

---

##  Tech Stack
**Frontend**
- [Next.js](https://nextjs.org/) (React framework)
- [Tailwind CSS](https://tailwindcss.com/) (styling)
- [Recharts](https://recharts.org/) (charts/graphs)

**Backend**
- [Django](https://www.djangoproject.com/) + [Django REST Framework](https://www.django-rest-framework.org/) (API)
- [PostgreSQL](https://www.postgresql.org/) (database)
- [pdfplumber](https://github.com/jsvine/pdfplumber) (PDF parsing)
- [ReportLab](https://www.reportlab.com/) (PDF reports)
- [OpenPyXL](https://openpyxl.readthedocs.io/) (Excel export)

**Deployment**
- [Vercel](https://vercel.com/) (frontend hosting)
- [Railway](https://railway.app/) / [Render](https://render.com/) (backend hosting)
- [Supabase](https://supabase.com/) or PostgreSQL cloud (database)

---

## 📂 Project Structure
```

bond-analysis-site/
│── frontend/       # Next.js app (UI, charts, pages)
│── backend/        # Django project (API, models, PDF parsing, reports)
│── database/       # DB migrations & setup
│── docs/           # Documentation, roadmap, ERD diagrams
│── README.md       # Project documentation

````

---

## ⚡ Getting Started

### 1️ Clone the repository
```bash
git clone https://github.com/<your-username>/bond-analysis-site.git
cd bond-analysis-site
````

### 2️ Frontend Setup (Next.js)

```bash
cd frontend
npm install
npm run dev
```

Visit → [http://localhost:3000](http://localhost:3000)

### 3️ Backend Setup (Django + PostgreSQL)

```bash
cd backend
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

API runs on → [http://localhost:8000](http://localhost:8000)

---

## Example Workflow

1. Upload a bond prospectus PDF.
2. System extracts bond details (coupon, maturity, tax, payment dates).
3. Enter investment amount (e.g., KES 2.5M).
4. View projected yearly and semi-annual returns.
5. Compare bonds side by side.
6. Download report as PDF/Excel.

---

##  Screenshots (to add later)

* Upload page
* Bond detail summary
* Calculator results with charts
* Comparison view
* PDF report sample

---

## Contributing

1. Fork this repo.
2. Create a feature branch: `git checkout -b feature/new-feature`
3. Commit changes: `git commit -m "Added new feature"`
4. Push branch: `git push origin feature/new-feature`
5. Submit a Pull Request.

---


## Acknowledgements

* Central Bank of Kenya (bond prospectuses)
* Django + Next.js community
* Open source libraries powering the project

---

