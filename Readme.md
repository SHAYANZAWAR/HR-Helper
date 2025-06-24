# HR Employee Records Agent

This project is an intelligent agent designed to help HR professionals interact with a database of employee records using natural language. It leverages Google Gemini (Generative AI) for language understanding and embeddings, and stores employee data in MongoDB Atlas with vector search capabilities.

## Features

- **Synthetic Employee Data Generation:** Automatically generates realistic employee records for testing and demonstration.
- **Natural Language Summaries:** Creates human-readable summaries of employee profiles.
- **Vector Search:** Uses Gemini embeddings to enable semantic search over employee records.
- **MongoDB Atlas Integration:** Stores and manages employee data in a scalable cloud database.

## Technologies Used

- [LangChain](https://js.langchain.com/) (Google Generative AI integration)
- [Google Gemini API](https://ai.google.dev/)
- [MongoDB Atlas](https://www.mongodb.com/atlas)
- [Zod](https://zod.dev/) (for schema validation)
- Node.js

## Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/your-repo.git
   cd agent
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Configure environment variables:**

   Create a `.env` file in the project root with the following content:
   ```
   GOOGLE_API_KEY=your-gemini-api-key
   MONGODB_URI=your-mongodb-atlas-uri
   ```

4. **Seed the database:**
   ```sh
   npx ts-node seed-database.ts
   ```

## Usage

After seeding, you can build agents or interfaces that query the employee database using semantic search and natural language, powered by Gemini embeddings.

## File Structure

- `seed-database.ts` – Generates synthetic employee data, summarizes it, and seeds MongoDB with vector search.
- `ReadMe.md` – Project documentation.

## License

MIT
