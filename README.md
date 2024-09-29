
# SQL Music Shop Database

This project creates a SQL database for managing a music shop, allowing for the storage and manipulation of data related to artists, albums, customers, employees, invoices, and tracks. It follows a relational database structure with tables connected through foreign keys to ensure data integrity and normalization.

## Database Structure

The database includes the following tables:

- **Artist**: Stores details of music artists (`artist_id`, `name`).
- **Album**: Links albums to artists (`album_id`, `title`, `artist_id`).
- **Employee**: Contains employee records, including management hierarchy via `reports_to`.
- **Customer**: Stores customer information, including the assigned support representative.
- **Genre**: Lists music genres.
- **Media Type**: Defines the types of media for tracks.
- **Track**: Stores track details like album, media type, genre, and pricing.
- **Playlist**: Holds playlists created by customers.
- **Playlist Track**: Links tracks to playlists.
- **Invoice**: Tracks customer purchases with billing information.
- **Invoice Line**: Provides details of each item on an invoice (track, price, and quantity).

## Key Features

- **Relational Integrity**: Enforces relationships between tables using foreign keys.
- **Employee Hierarchy**: Employees can report to a manager (`reports_to`).
- **Comprehensive Music Data**: Tracks can be categorized by genre, media type, and album.
- **Invoice System**: Customers can purchase tracks, and invoices are generated with detailed line items.

