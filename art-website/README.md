# Art Website

This project is an art website built using Svelte and TypeScript. It showcases various artworks and provides a user-friendly interface for navigation.

## Project Structure

```
art-website
├── src
│   ├── components
│   │   └── Header.svelte       # Svelte component for the website header
│   ├── pages
│   │   └── Home.svelte         # Main home page displaying featured artworks
│   ├── styles
│   │   └── main.css            # CSS styles for the website
│   └── main.ts                 # Entry point of the application
├── public
│   └── index.html              # Main HTML file serving the application
├── package.json                 # npm configuration file
├── tsconfig.json               # TypeScript configuration file
└── README.md                   # Documentation for the project
```

## Setup Instructions

1. Clone the repository:
   ```
   git clone <repository-url>
   cd art-website
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Run the application:
   ```
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5000` to view the website.

## Features

- Responsive design for various devices
- Dynamic content display for artworks
- Easy navigation through the header component

## Usage Guidelines

- Modify the `src/pages/Home.svelte` file to update the main content of the home page.
- Customize styles in `src/styles/main.css` to change the look and feel of the website.
- Add new components in the `src/components` directory as needed.

## License

This project is licensed under the MIT License.