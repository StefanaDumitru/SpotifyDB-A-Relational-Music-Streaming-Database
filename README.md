# SpotifyDB: A Relational Music Streaming Database

A structured SQL-based relational database that models the backend for a music streaming platform, inspired by Spotify. This project includes entities such as bands, artists, albums, songs, categories, and composers, with all appropriate relationships and constraints.

## 📁 Project Structure

- proiectBD.sql: Main SQL script containing:
  - Database creation and selection
  - Table definitions with primary and foreign keys
  - Sample schema for a music platform

## 🛠 Technologies Used

- MySQL / MariaDB
- SQL DDL (Data Definition Language)

## 🧱 Database Schema Overview

The database includes the following main entities:

- *tblBands* – Contains information about music bands (name, members, origin, etc.)
- *tblArtists* – Stores individual artists related to bands
- *tblAlbums* – Albums produced by bands, linked to songs
- *tblSongs* – Songs linked to albums and categories
- *tblCategories* – Song categories or genres (e.g., Rock, Pop)
- *tblComposers* – Details about the composers for each song

### Entity Relationships

- A band can have many albums and artists.
- An album contains multiple songs.
- A song belongs to one category and is composed by one or more composers.
- Composers are associated with both bands and songs.

## 🚀 How to Use

1. Clone the repository or download the proiectBD.sql file.
2. Open your MySQL/MariaDB client.
3. Run the script:
   ```sql
   SOURCE path/to/proiectBD.sql;
