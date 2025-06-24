# My Own Custom File-Based Database 

A simple, file-based JSON database implemented in Go. This project demonstrates how to create, read, update, and delete user records stored as JSON files, using basic concurrency control and logging.

## Features

- Store user data as JSON files in a directory structure.
- CRUD operations: Create, Read, Update, Delete.
- Thread-safe operations using mutexes.
- Simple logging using [lumber](https://github.com/jcelliott/lumber).
- Example user data and usage in `main.go`.

## Project Structure

```
.
├── main.go         # Main application and database logic
├── users/          # Directory containing user JSON files
│   ├── Ashutosh.json
│   ├── Ashyam.json
│   ├── Kartikey.json
│   ├── Mayank.json
│   ├── Nitesh.json
│   └── Sparsh.json
```

## Usage

1. **Install dependencies**  
   Make sure you have Go installed.  
   Install the lumber logger:
   ```
   go get github.com/jcelliott/lumber
   ```

2. **Run the application**
   ```
   go mod tidy
   go run main.go
   ```

3. **Modify or extend**  
   - Add or update user data in the `users` directory.
   - Modify the `main.go` logic for more features.

## Example

The application will:
- Write a set of user records to the `users` directory.
- Read all users and print them to the console.

## License

MIT License
