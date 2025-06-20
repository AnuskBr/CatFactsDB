# CatFactsDB 🐱

**CatFactsDB** is a multimedia database project designed to organize and provide centralized access to information about cat breeds. It combines classical data (like breed names, traits, and diseases) with rich multimedia content such as images, videos, audio files, texts, posters, and presentations — all integrated within a unified PostgreSQL relational database structure.

## 📌 Project Overview

Cats have played a symbolic and emotional role in human history, from Ancient Egypt to today’s modern homes. With the vast diversity of cat breeds and the dispersed nature of information online, CatFactsDB was created to address the need for a centralized, multimedia-rich resource that offers complete, interactive insights into cat breeds.

The application is targeted at cat lovers, pet owners, and anyone seeking to explore feline-related data in a structured, efficient, and visually engaging way.

## 🧩 Features

- Stores descriptive data on cat breeds, traits, and associated diseases.
- Organizes multimedia content: videos, audio clips, photos, texts, posters, and presentations.
- Utilizes metadata for technical, contextual, and content-based descriptions.
- Provides an easy querying mechanism using SQL for information retrieval.
- Includes support for compound media objects (e.g., a poster made of text and images).

## 🛠️ Technologies Used

- **PostgreSQL** – Relational database system
- **PgAdmin 4** – GUI for database management
- **SQL** – For database creation and data querying
- **JSON** – Used for storing metadata about media equipment

## 🗃️ Database Structure

### Main Entity Groups:

1. **Descriptive Entities**
   - `Rase_pisici`: Cat breed names
   - `Caracteristici`: Physical and behavioral traits
   - `Boli`: Associated illnesses

2. **Simple Media Objects**
   - `Videouri`, `Audiouri`, `Imagini`, `Texte`: Each contains metadata about file format, size, content, and origin

3. **Compound Media Objects**
   - `Inregistrari`: Contain both video and audio
   - `Prezentari`: Contain video, audio, and text
   - `Postere`: Contain images and text

4. **Metadata Equipment**
   - `Echipamente`: Stores device-related metadata (e.g., camera model, microphone specs) in JSON format


## 🔍 Example Queries

- Display all texts about breeds like Maine Coon, Bengal, and Scottish Fold that mention keywords such as "food", "HCM", or "origin".
- Retrieve all recordings involving the Bengal breed.
- List posters about Cymric cats and their food habits.
- Show presentations filmed with GoPro devices involving Scottish Fold cats.
- List all characteristics of the American Shorthair breed.

---

> This project was created as part of a multimedia databases course to demonstrate advanced entity modeling and metadata integration using PostgreSQL.

