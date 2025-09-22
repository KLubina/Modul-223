# **DKSynergy Hotel Management System**

## **Projektbeschreibung**  
Dieses **Hotelbuchungssystem** ermöglicht es **Benutzern**, Zimmer zu durchsuchen, zu buchen und Buchungen zu verwalten. **Admins** können Zimmer hinzufügen, bearbeiten und Buchungen verwalten.  

## **Technologien**  
### **Backend:**  
- Java (Spring Boot)  
- PostgreSQL / MongoDB  
- Spring Security (JWT-Authentifizierung)  
- AWS S3 (für Bilder-Uploads)  

### **Frontend:**  
- React (mit Vite)  
- React Router  
- Axios (für API-Requests)  

---

## **Installation & Setup**  

### **Backend starten:**  
1. **Projekt klonen:**  

   git clone <repo-url>
   cd DKSynergy-backend

2. **Datenbank konfigurieren** (in `application.properties` oder `application.yml`).  
3. **Abhängigkeiten installieren & starten:**  
 
   mvn install
   mvn spring-boot:run

4. **API testen:** Öffne Postman und rufe `http://localhost:4040/api` auf.  

---

### **Frontend starten:**  
1. **In das Frontend wechseln:** 

   cd ../dksynergy-hotel-react
   
2. **Abhängigkeiten installieren:**  

   npm install

3. **Entwicklungsserver starten:**  
   npm run dev
4. **Frontend im Browser öffnen:**  
   `http://localhost:5173`  

---

## **Funktionen**  
### **Benutzer:**  
✅ Registrierung & Login  
✅ Zimmer suchen & buchen  
✅ Buchungshistorie ansehen  
✅ Buchung per Bestätigungscode finden  

### **Admin:**  
✅ Zimmer verwalten (Hinzufügen, Bearbeiten, Löschen)  
✅ Buchungen verwalten (Abschließen, Stornieren)  
✅ Benutzer verwalten  

---

## **API-Endpunkte (Backend)**  
| **Methode** | **Endpoint**               | **Beschreibung**             |
|------------|----------------------------|-----------------------------|
| **POST**   | `/auth/register`            | Benutzer registrieren       |
| **POST**   | `/auth/login`               | Benutzer einloggen          |
| **GET**    | `/users/get-logged-in-profile-info` | Benutzerprofil abrufen  |
| **GET**    | `/rooms/all`                | Alle Zimmer abrufen         |
| **POST**   | `/rooms/add`                | Neues Zimmer hinzufügen (Admin)  |
| **POST**   | `/bookings/book-room/{roomId}/{userId}` | Zimmer buchen |

➡️ **Weitere Endpunkte sind im Code dokumentiert.**  

---

## **Autoren**  
📌 **Autoren:** Daniel Kovac & Kristian Lubina
