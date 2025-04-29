# LinkSnip URL Shortener

LinkSnip is a modern, lightweight URL shortener service built with pure JavaScript. It allows users to create shortened URLs with custom short codes and manage their links through a sleek, responsive interface.

![LinkSnip Screenshot](/image.png)

## Features

- **Custom URL Shortening**: Create shortened URLs with personalized short codes
- **Copy and Share**: Easily copy shortened links with a single click
- **Responsive Design**: Modern UI that works across all device sizes
- **Real-time Updates**: Instantly see your shortened URLs without page refresh
- **Persistent Storage**: Links are stored in a JSON file for persistence

## Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend**: Node.js with native HTTP module
- **Data Storage**: File-based storage using Node.js fs/promises
- **Styling**: Custom CSS with responsive design and animations
- **Icons**: Font Awesome for UI elements

## Technical Implementation Details

- **Server-side Routing**: Implemented a custom router using Node.js native HTTP server to handle different endpoints without using Express
- **File-based Persistence**: Created a data storage system using JSON files and async/await pattern for handling file operations
- **Modern UI Components**: Built custom notification system, form validation, and interactive elements with pure JavaScript
- **Cryptographic Short Codes**: Implemented random short code generation using Node.js crypto module
- **Responsive Design**: Created a fully responsive UI with support for mobile devices down to 320px width

Here's the combined markdown file content based on the two images you provided:
## Installation & Setup

1. Clone the repository:  
   ```bash
   git clone https://github.com/adityapandey7/URLShortner.git
   cd URLShortner
   ```

2. Make sure you have Node.js installed (v14+ recommended)

3. Create a data directory for storing links:
   ```bash
   mkdir -p data
   ```

4. Run the server:
   ```bash
   node app.js
   ```

5. Open your browser and navigate to:
   ```
   http://localhost:3002
   ```

## Project Structure

```
URLShortner/
├── app.js                 # Main server file
├── public/
│   ├── index.html         # Main HTML file
│   └── style.css          # CSS styles
├── data/
│   └── link.json          # JSON file for storing links
└── README.md              # Project documentation
```

## How It Works

1. The server runs on Node.js and handles both the web interface and API endpoints
2. When a user submits a URL with a custom short code, it's saved to the link.json file
3. When someone visits a shortened URL, the server looks up the original URL and redirects
4. The UI is designed to be intuitive with real-time feedback and copy functionality

## Future Improvements

- Add user authentication
- Implement link analytics (click tracking)
- Add expiration dates for links
- Create API documentation for programmatic access
- Add custom QR code generation for links