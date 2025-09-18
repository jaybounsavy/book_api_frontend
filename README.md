# Book Management System - Frontend

This is the HTML frontend application for the Book API that provides a user-friendly interface to manage books.

## Features

- 📚 **Display Books**: View all books in a responsive table format
- ➕ **Add Books**: Form to add new books to the database
- 🗑️ **Delete Books**: Remove books with confirmation dialog
- 🎨 **Bootstrap Styling**: Modern, responsive UI with Bootstrap CSS
- 🔄 **Real-time Updates**: Automatic refresh after add/delete operations
- ⚠️ **Error Handling**: Graceful handling of API connection issues with sample data
- 📱 **Mobile Responsive**: Works on all device sizes

## API Endpoint

The application connects to: `https://bookapi-jbounsa-g6d0f0gsc8cee9em.centralus-01.azurewebsites.net/api/books/`

## Quick Start

### Option 1: Direct File Access
Simply open `index.html` in your web browser.

### Option 2: Local Server (Recommended)
For better CORS handling and testing:

```bash
# Using Python 3
python3 server.py

# Or using Python 2
python server.py
```

Then open your browser to `http://localhost:8000`

### Option 3: Alternative Servers
```bash
# Using Node.js http-server (if installed)
npx http-server

# Using PHP (if installed)
php -S localhost:8000
```

## Book Data Structure

The application expects books to have the following structure:

```json
{
  "id": 1,
  "title": "Book Title",
  "author": "Author Name", 
  "isbn": "978-0-123-45678-9",
  "genre": "Fiction",
  "publishedYear": 2023,
  "description": "Book description..."
}
```

## Technical Details

- **Frontend**: Pure HTML, CSS (Bootstrap 5.3), JavaScript (ES6+)
- **API Integration**: Fetch API for HTTP requests
- **Styling**: Bootstrap 5.3 with Bootstrap Icons
- **Responsive Design**: Mobile-first approach
- **Error Handling**: Fallback to sample data when API is unavailable

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- All modern browsers that support ES6 features

## Troubleshooting

1. **CORS Issues**: Use the provided `server.py` or any local server instead of opening the file directly
2. **API Connection**: If the API is down, the app will show sample data with a warning
3. **Form Validation**: Required fields (Title and Author) must be filled before submission

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request
