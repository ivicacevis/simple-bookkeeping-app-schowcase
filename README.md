# Simple Bookkeeping App Showcase

**Simple Bookkeeping App Showcase** — a private Django project built for managing finances in associations.  
It includes role-based access, data validation, Croatian localization, PDF export, HTMX modals, and DataTables integration.  
This repo is a portfolio showcase of the main features.

---

## ✨ Overview
This showcase highlights a private bookkeeping project developed with Django.  
The goal was to create a simple, secure, and user-friendly system for associations and small organizations.

---

## 🔧 Technologies Used
- **Backend**: Django, Django REST Framework, PostgreSQL  
- **Async Tasks**: Celery + Redis  
- **Server**: Daphne (ASGI) behind Nginx  
- **Frontend**: Django Templates, Bootstrap, HTMX, DataTables  
- **PDF Export**: WeasyPrint (HTML + Jinja → PDF)  
- **Deployment**: Ubuntu server, `.env` configs, Gmail SMTP for emails  

---

## 📊 Features
- Custom user model with roles: **admin, manager, client, member**  
- Role-based access control with [django-rules](https://github.com/dfunckt/django-rules)  
- Two-factor authentication (MFA via email code)  
- Association & Year management (active / archived)  
- Bookkeeping modules:
  - Cashflows (cash book)  
  - Incomes & Outcomes (income/expense book)  
  - In/Out Receipts  
  - Revenues, Payins, Payouts  
  - Assets, Travels (travel orders & expenses)  
  - Payment Orders (HUB-3A PDF with barcode)  
- Interactive tables (DataTables) with filtering & Croatian localization  
- Dynamic CRUD with **HTMX modals**  
- PDF reports with localized date & number formatting (d.m.yyyy. / 1.234,56 €)  

---

## 📸 Screenshots
> *(to be added – insert app screenshots or GIFs here to demonstrate UI and features)*

---

## 📖 Lessons Learned
- Importance of **backend-first validation** with frontend fallbacks  
- Benefits of **monolithic Django architecture** for maintainability  
- Reusable approach for **modular apps** (each with forms, views, templates, JS validation)  
- Handling **Croatian localization** for dates and numbers across frontend, backend, and exports  

---

## 🚀 Next Steps
- Extract reusable parts as open-source packages (e.g. PDF export utilities, Croatian decimal/date fields)  
- Expand showcase with demo modules and example code snippets  

---
