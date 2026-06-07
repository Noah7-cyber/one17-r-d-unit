# R&D Unit Vue App

This project is a Vue.js conversion of the R&D Unit single-page dashboard. It utilizes Vite for fast development and bundling.

## Setup Instructions

1. **Install Dependencies**
   Make sure you have Node.js installed. In the root directory of this project, run:
   ```bash
   npm install
   ```

2. **Start the Development Server**
   Run the following command to start Vite's local development server:
   ```bash
   npm run dev
   ```
   Open the local URL provided in your terminal in your browser to view the app.

3. **Build for Production**
   To build the app for production, run:
   ```bash
   npm run build
   ```
   The compiled assets will be placed in the `dist` folder.

4. **Preview the Production Build**
   To test the production build locally, run:
   ```bash
   npm run preview
   ```

## Notes
- This is a vanilla JavaScript Vue 3 project using `<script setup>` syntax (no TypeScript).
- Original CSS styles from the HTML template are preserved in `src/assets/main.css` and imported globally.
- The dashboard is broken down into modular components within the `src/components` directory.