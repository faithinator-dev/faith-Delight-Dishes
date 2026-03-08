# Faith Delight Dishes

A modern, responsive food discovery website that allows users to explore traditional African dishes. The application fetches data from a custom API and provides advanced filtering, searching, and detailed views for each dish.

## 🌟 Features

- **Dynamic Content**: Fetches food data dynamically from an external API.
- **Smart Filtering**:
  - Filter by **Category** (Main Dishes, Soups, Swallows, Snacks, etc.).
  - Filter by **Region** (South-West, South-East, Northern, South-South Nigeria).
  - Toggle filters for **Vegetarian** and **Spicy** options.
- **Real-time Search**: Instantly find dishes by name as you type.
- **Interactive UI**:
  - **Hero Carousel**: Randomly highlights 3 popular dishes on every page load.
  - **Modal Details**: Click "Show Details" to see ingredients, preparation steps, calories, and difficulty.
- **Favorites System**: Save your favorite dishes to a list (persisted using LocalStorage).
- **Responsive Design**: Built with Bootstrap 5 for a seamless experience on mobile and desktop.
- **Error Handling**: User-friendly loading states and error messages if the API fails.

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Framework**: Bootstrap 5.3.8 (CSS & JS Bundle)
- **Icons**: FontAwesome 6.5.0
- **Data Source**: Custom REST API (`https://mongotest2026.vercel.app/api/foods`)

## 🚀 How to Run

1. **Clone the repository** or download the source code.
2. Ensure you have an internet connection (required to fetch data from the API and load CDN resources).
3. Open `index.html` in your web browser.
   - *Note: `index.html` contains the latest modern UI with the carousel and improved logic.*

## 📂 Project Structure

- `index.html`: The main entry point with the modern UI, carousel, and advanced filtering logic.
- `bin/`: Contains backup or reference files.
- `bin/index2.html`: An alternative/older version of the layout.
- `*.jpg`: Local image assets used as fallbacks or mapped to specific food IDs.

## 🧩 Logic Overview

- **Data Fetching**: Uses `async/await` to fetch data. Includes a loading spinner and error retry button.
- **Image Mapping**: Since the API might lack images, a local array maps food IDs to local `.jpg` files.
- **State Management**: All data is stored in a global `allFoods` array to allow instant filtering without re-fetching.
- **Local Storage**: The "Favorites" list is saved in the browser's LocalStorage so data isn't lost on refresh.

---

*Created for the SQI JavaScript october cohort level one javascript class as a final project.*
