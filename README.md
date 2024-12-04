# WebDiaryAPI 📖

WebDiaryAPI is a RESTful API built using ASP.NET Core. It provides endpoints to perform CRUD operations (Create, Read, Update, Delete) for managing diary entries.

---

## Features 🚀

- **GET**: Fetch all diary entries or retrieve a specific entry by ID.
- **POST**: Create new diary entries.
- **PUT**: Update existing diary entries.
- **DELETE**: Remove diary entries.

---

## API Endpoints 🌐

### **DiaryEntries**

| Method   | Endpoint                | Description                      |
|----------|-------------------------|----------------------------------|
| **GET**  | `/api/DiaryEntries`     | Retrieve all diary entries.      |
| **GET**  | `/api/DiaryEntries/{id}`| Retrieve a single entry by ID.   |
| **POST** | `/api/DiaryEntries`     | Create a new diary entry.        |
| **PUT**  | `/api/DiaryEntries/{id}`| Update an existing entry by ID.  |
| **DELETE**| `/api/DiaryEntries/{id}`| Delete a diary entry by ID.      |

---

## Project Structure 📂

- **Controllers**: Includes `DiaryEntriesController.cs`, which handles API requests.
- **Models**: Contains `DiaryEntry.cs`, the data model for diary entries.
- **Data**: Contains `ApplicationDbContext.cs`, which manages the database connection and entity configurations.

---

## Technologies and Tools 🛠️

- **ASP.NET Core Web API**: Framework for building the API.
- **Entity Framework Core**: For data access and database operations.
- **Swagger**: Integrated for API documentation and testing.
- **C#**: Programming language.

---

## Running the API 🖥️

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your_username/WebDiaryAPI.git
   cd WebDiaryAPI
   ```

2. **Install dependencies**:  
   Open the project in Visual Studio and ensure all NuGet packages are installed.

3. **Apply database migrations**:
   Run the command:
   ```bash
   dotnet ef database update
   ```

4. **Run the application**:  
   Use Visual Studio or execute:
   ```bash
   dotnet run
   ```

5. **Access the Swagger UI**:  
   Once the API is running, open your browser and go to:  
   ```
   http://localhost:<port>/swagger
   ```
   Here, you can explore and test all available endpoints.

---

## Database Structure 🗃️

The `DiaryEntries` table includes:
- **Id**: Primary key.
- **Title**: Entry title.
- **Content**: Entry content.
- **Date**: Entry date.

---

## Author 📌

- **Name/Nickname**: Mikołaj Winkiel
- **License**: MIT

---
