# 🌾 AgriSmart ---- Fertilizer Recommendation System

A smart, AI-powered application that recommends the most suitable fertilizers for farmers. It works in two modes:

1. **Soil Report-Based Recommendation** – Uses a Machine Learning model (Random Forest) trained with Scikit-learn.
2. **Location-Based Recommendation** – Uses Google's **Gemini API** based on location, crop, season, and soil type.

---

## 🚀 Features

- 🧪 Accepts detailed soil reports and predicts optimal fertilizers using ML.
- 📍 Uses Gemini API for farmers who don't know soil data, by analyzing location + crop data.
- 🔐 Clerk-based user authentication.
- 📊 Data visualization with Recharts.
- 🌐 Seamless, fast frontend with React + Vite + TypeScript.

---

## 🛠 Tech Stack

### Frontend

| Feature             | Tech                                                                 |
|---------------------|----------------------------------------------------------------------|
| Framework           | [React](https://reactjs.org/) + [TypeScript](https://www.typescriptlang.org/) |
| Build Tool          | [Vite](https://vitejs.dev/)                                          |
| UI Libraries        | [shadcn-ui](https://ui.shadcn.com/), [Radix UI](https://www.radix-ui.com/), [Tailwind CSS](https://tailwindcss.com/) |
| State Management    | React Hooks                                                          |
| Authentication      | [Clerk](https://clerk.dev/)                                          |
| Routing             | [React Router DOM](https://reactrouter.com/)                         |
| Forms & Validation  | [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/) |
| Data Visualization  | [Recharts](https://recharts.org/)                                    |
| HTTP Client         | [Axios](https://axios-http.com/)                                     |
| API Integration     | [TanStack React Query](https://tanstack.com/query/latest)            |

> **Backend:** This project does connects to external APIs like Gemini and optionally a hosted ML model.

---

## 🧠 How It Works

### 1. Soil-Based Recommendation (Machine Learning)
- **Input:** N, P, K, pH, Moisture, Humidity, Temperature, Crop.
- **Output:** A recommended fertilizer based on Random Forest classification.

### 2. Location-Based Recommendation (Gemini API)
- **Input:** Location, Crop Type, Soil Type, Season.
- **Output:** AI-generated fertilizer suggestions from Gemini API.


## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/fertilizer-recommendation-system.git
cd fertilizer-recommendation-system


cd Frontend
npm install


# Clerk Authentication
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here

# Gemini API backend proxy (recommended to protect API key)
VITE_GEMINI_BACKEND_URL=https://your-serverless-or-backend.com/gemini

# ML Model API URL (optional if using soil analysis)
VITE_ML_MODEL_API_URL=https://your-flask-ml-api.com/predict

# Optional Base URL
VITE_API_BASE_URL=https://your-api-base-url.com

# Optional Metadata
VITE_APP_NAME=Fertilizer Recommender
VITE_NODE_ENV=development


# Clerk Authentication
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here

# Gemini API backend proxy (recommended to protect API key)
VITE_GEMINI_BACKEND_URL=https://your-serverless-or-backend.com/gemini

# ML Model API URL (optional if using soil analysis)
VITE_ML_MODEL_API_URL=https://your-flask-ml-api.com/predict

# Optional Base URL
VITE_API_BASE_URL=https://your-api-base-url.com

# Optional Metadata
VITE_APP_NAME=Fertilizer Recommender
VITE_NODE_ENV=development

