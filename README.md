# Simple Bookkeeping App Showcase

**Simple Bookkeeping App Showcase** — a private Django project built for managing finances in associations.  
It includes role-based access, data validation, Croatian localization, PDF export and DataTables integration.  
This repo is a portfolio showcase of the main features.

---
https://jednostavno-knjigovodstvo.hr/
## ✨ Overview
This showcase highlights a private bookkeeping project developed with Django.  
The goal was to create a simple, secure, and user-friendly system for associations and small organizations.

---

## 🔧 Technologies Used
- **Backend**: Django, Django REST Framework, PostgreSQL  
- **Async Tasks**: Celery + Redis  
- **Server**: Daphne (ASGI) behind Nginx  
- **Frontend**: Django Templates, Bootstrap, DataTables  
- **PDF Export**: WeasyPrint (HTML + Jinja → PDF)  
- **Deployment**: Ubuntu server, `.env` configs, 

---

## 📊 Features
- Custom user model with roles: **admin, manager, client, member**  
- Role-based access control with [django-rules](https://github.com/dfunckt/django-rules)  
- Two-factor authentication (MFA via email code)  
- Association & Year management (active / archived)  
- Bookkeeping modules:
  - Knjiga blagajne  
  - Knjiga primitaka i izdataka 
  - Knjiga ulaznih računa / Knjiga izlaznih računa
  - Evidencija o prihodima
  - Uplatnice / Isplatnice
  - Popis imovine  
  - Putni nalozi (troškovi, vozila, putnici)  
  - Platni nalozi (HUB-3A PDF s barkodom)  
- Interactive tables (DataTables) with filtering & Croatian localization  
- Dynamic CRUD 
- PDF reports with localized date & number formatting (d.m.yyyy. / 1.234,56 €)  

---

## 📸 Screenshots
<img width="1331" height="800" alt="image" src="https://github.com/user-attachments/assets/739cee94-a715-4b51-88e8-bff6ae5e3c2c" />
<img width="1336" height="522" alt="image" src="https://github.com/user-attachments/assets/78428159-83c8-4440-b415-9184607f9bfa" />
<img width="1343" height="553" alt="image" src="https://github.com/user-attachments/assets/b8a35f93-5611-4744-bd98-9dc006ce1d7f" />
<img width="1353" height="461" alt="image" src="https://github.com/user-attachments/assets/85166f0f-4bef-42bd-b1fe-87e1f330f0b1" />
<img width="1354" height="903" alt="image" src="https://github.com/user-attachments/assets/bc8e3058-23e3-4bb3-bfa0-40d5afdd25f4" />
<img width="1357" height="749" alt="image" src="https://github.com/user-attachments/assets/ae796ae7-18a8-49c7-b9a2-07f05cbd9253" />
<img width="1435" height="560" alt="image" src="https://github.com/user-attachments/assets/f838b3be-5280-4cc9-a4cc-fd26e1c8a790" />


---

## 📖 Lessons Learned
- Importance of **backend-first validation** with frontend fallbacks  
- Benefits of **monolithic Django architecture** for maintainability  
- Reusable approach for **modular apps** (each with forms, views, templates, JS validation)  
- Handling **Croatian localization** for dates and numbers across frontend, backend, and exports  

---
