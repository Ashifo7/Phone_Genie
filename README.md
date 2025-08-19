# 📱 PhoneGenie - Smartphone Recommendation Engine

PhoneGenie is an intelligent web application that helps users find their perfect smartphone based on personal preferences, budget, and usage patterns. Powered by machine learning, it provides personalized phone recommendations and predicts device viability.

## ✨ Features

- **Personalized Recommendations**: Get phone suggestions tailored to your preferences
- **Viability Prediction**: Predict how long a phone will remain usable
- **Interactive Comparison**: Compare multiple phones side-by-side
- **Smart Filters**: Filter by price range, brand, and specifications
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Dark/Light Mode**: Choose your preferred theme

## 🚀 Tech Stack

### Frontend
- React 18 with TypeScript
- Vite (Build Tool)
- Tailwind CSS (Styling)
- Recharts (Data Visualization)
- React Context API (State Management)

### Backend
- Python 3.8+
- Flask (Web Framework)
- Scikit-learn (Machine Learning)
- Joblib (Model Persistence)

### Machine Learning Models
- **Recommendation Model**: Random Forest Regressor for personalized phone suggestions
- **Viability Model**: Gradient Boosting Regressor for predicting phone longevity

## 🛠️ Installation

### Prerequisites
- Node.js (v16+)
- Python 3.8+
- pip (Python package manager)

### Setup

1. **Clone the repository**
   ```bash
   git clone [(https://github.com/Ashifo7/Phone_Genie)](https://github.com/Ashifo7/Phone_Genie)
   cd PhoneGenie
   ```

2. **Set up the backend**
   ```bash
   # Create and activate virtual environment
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate

   # Install Python dependencies
   pip install -r requirements.txt
   ```

3. **Set up the frontend**
   ```bash
   cd frontend
   npm install
   ```

## 🚦 Running the Application

### Development Mode

1. **Start the backend server**
   ```bash
   # From project root
   python app.py
   ```

2. **Start the frontend development server**
   ```bash
   # From frontend directory
   npm run dev
   ```

3. Open [http://localhost:3000](http://localhost:3000) in your browser

### Production Build

1. Build the frontend:
   ```bash
   cd frontend
   npm run build
   ```

2. The production build will be in the `dist` directory

## 🤖 Machine Learning Models

### Training the Models

1. **Recommendation Model**
   - Trains on user preferences and phone specifications
   - Updates with user feedback for continuous improvement

2. **Viability Model**
   - Predicts phone longevity based on specifications and historical data
   - Continuously improves with new data

### Model Persistence
- Models are automatically saved in `ml/models/saved/`
- Includes both the model and its feature scaler

## 🌐 API Endpoints

- `GET /api/recommendations` - Get phone recommendations
- `POST /api/feedback` - Submit feedback on recommendations
- `GET /api/viability` - Get phone viability prediction

## 📊 Data

Phone specifications and user preferences are stored in:
- `src/data/phones.ts` - Phone specifications database
- `src/types/phone.ts` - TypeScript interfaces for phone data

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with ❤️ by [Your Name]
- Icons by [Lucide Icons](https://lucide.dev/)
- Phone data from various public sources
