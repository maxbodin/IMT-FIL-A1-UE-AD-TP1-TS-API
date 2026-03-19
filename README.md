# IMT-FIL-A1-UE-AD-TP1-TS-API - Todo Lists API

REST API for managing todo lists and items, built with [Fastify](https://fastify.dev) and TypeScript. Uses LevelDB for efficient, persistent data storage.

## Features

- Full CRUD operations for todo lists.
- Manage items within lists (create, read, update, delete).
- LevelDB persistence for fast, scalable storage.
- TypeScript for type safety.
- Comprehensive test coverage.
- Auto-loaded plugins and routes.

## API Endpoints

### Lists
- `GET /` - Get all lists.
- `POST /` - Create a new list.
- `GET /:id` - Get a specific list.
- `PUT /:id` - Update a list.
- `DELETE /:id` - Delete a list.

### Items
- `GET /:id/items` - Get all items in a list.
- `POST /:id/items` - Add an item to a list.
- `PUT /:id/items/:itemId` - Update an item.
- `DELETE /:id/items/:itemId` - Delete an item.

## Quick Start

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

Starts the app in watch mode at `http://localhost:3000`

### Production

```bash
npm start
```

### Testing

```bash
npm run test
```

## Project Structure

```
src/
├── app.ts                 # Main application
├── controllers/           # Request handlers
├── routes/               # API endpoints
├── plugins/              # Fastify plugins (LevelDB, sensible, support)
├── interfaces/           # TypeScript interfaces
└── schema/              # JSON schemas
```