![JavaScript Badge](https://img.shields.io/badge/language-JavaScript-yellow.svg)
![Express.js Badge](https://img.shields.io/badge/framework-Express.js-brightgreen.svg)

# Notes-Express-api 📝

This repository contains a learning project focused on building a Notes API using Express.js. It serves as a practical demonstration of fundamental backend development concepts with Node.js and Express.

## 🚀 Features

*   **RESTful API Design:** Implements standard HTTP methods (GET, POST, PUT, DELETE) for managing notes.
*   **CRUD Operations:** Supports Create, Read, Update, and Delete operations for notes.
*   **Data Persistence (In-memory):** Utilizes an in-memory array for storing notes during the learning phase.
*   **Unique ID Generation:** Employs `nanoid` for generating unique identifiers for each note.
*   **Cross-Origin Resource Sharing (CORS):** Configured to allow requests from different origins.
*   **Development Server:** Uses `nodemon` for automatic server restarts during development.
*   **Linting and Formatting:** Integrates ESLint for code quality and consistency.

## 💡 Installation

To get started with this project, clone the repository and install the necessary dependencies.

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/Rizald95/Notes-Express-api.git
    cd Notes-Express-api
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    ```

## ▶️ Usage

Once the dependencies are installed, you can start the development server.

1.  **Start the development server:**

    ```bash
    npm run dev
    ```

    This command will start the server, typically on `http://localhost:5000` (or the port specified in `src/server.js`).

2.  **API Endpoints:**

    *   **`GET /notes`**: Retrieve all notes.
    *   **`GET /notes/:id`**: Retrieve a specific note by its ID.
    *   **`POST /notes`**: Create a new note. The request body should be a JSON object with a `title` and `body` property.
    *   **`PUT /notes/:id`**: Update an existing note by its ID. The request body should be a JSON object with the properties to update.
    *   **`DELETE /notes/:id`**: Delete a note by its ID.

### Example Requests (using `curl`)

**Create a new note:**

```bash
curl -X POST -H "Content-Type: application/json" -d '{"title": "Learning Express", "body": "This is a note about learning Express.js"}' http://localhost:5000/notes
```

**Get all notes:**

```bash
curl http://localhost:5000/notes
```

**Get a specific note (replace `your_note_id` with an actual ID):**

```bash
curl http://localhost:5000/notes/your_note_id
```

**Update a note (replace `your_note_id` with an actual ID):**

```bash
curl -X PUT -H "Content-Type: application/json" -d '{"title": "Updated Learning Express", "body": "Updated content of the note"}' http://localhost:5000/notes/your_note_id
```

**Delete a note (replace `your_note_id` with an actual ID):**

```bash
curl -X DELETE http://localhost:5000/notes/your_note_id
```

## 🤝 Contributing

As this is a learning project, contributions are welcome in the form of suggestions, bug reports, or pull requests that enhance the learning experience or code quality.

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature`).
3.  Commit your changes (`git commit -m 'Add some feature'`).
4.  Push to the branch (`git push origin feature/your-feature`).
5.  Open a Pull Request.

## 📜 License

This project does not currently have a specified license.

---

<p align="center">
  <a href="https://readmeforge.app?utm_source=badge">
    <img src="https://readmeforge.app/badge.svg" alt="Made with ReadmeForge" height="20">
  </a>
</p>