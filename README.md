# Calorie Tracker App

A comprehensive React Native calorie tracking application with BMI calculation, image recognition, manual logging, and barcode detection.

## Features

### 🏠 **Home Dashboard**
- Personalized welcome screen with user profile
- BMI display with color-coded categories
- Daily calorie progress tracking
- Nutrient breakdown (protein, carbs, fat)
- Quick action buttons for easy navigation
- Recent food entries overview

### 📊 **BMI Calculator**
- Complete user profile creation
- Automatic BMI calculation and categorization
- Daily calorie needs estimation using Mifflin-St Jeor equation
- Activity level selection (sedentary to very active)
- Profile saving and management

### 📷 **Image Recognition**
- Camera integration for food photography
- AI-powered food detection and calorie estimation
- Support for both camera capture and gallery selection
- Automatic nutritional information extraction
- Confidence scoring for detected foods

### ✍️ **Manual Food Logging**
- Smart food name recognition
- Quantity input with multiple units (g, kg, ml, cups, etc.)
- Automatic nutrient estimation based on food categories
- Meal type categorization (breakfast, lunch, dinner, snack)
- Real-time nutritional calculations

### 📱 **Barcode Scanner**
- Real-time barcode scanning
- Comprehensive food database integration
- Automatic product recognition and nutritional data
- Support for multiple barcode formats (EAN13, EAN8, UPC, Code128, etc.)
- Sample product database included

### 📈 **History & Analytics**
- Complete food log history
- Time-based filtering (week, month, all)
- Daily nutritional summaries
- Calorie and nutrient tracking over time
- Visual progress indicators

### 👤 **Profile Management**
- User profile with BMI information
- Activity level tracking
- Personal statistics and streaks
- Quick access to all app features
- Data management options

## Technical Features

### 🗄️ **Database**
- SQLite local database for offline functionality
- Comprehensive data models for users, food items, and logs
- Efficient data storage and retrieval
- Sample food database with common products

### 🎨 **UI/UX**
- Modern Material Design interface
- Intuitive navigation with bottom tabs
- Responsive design for all screen sizes
- Color-coded BMI categories
- Progress indicators and visual feedback

### 📱 **Platform Support**
- Cross-platform React Native implementation
- Android and iOS compatibility
- Native camera and barcode scanning
- Platform-specific optimizations

## Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- React Native CLI
- Android Studio (for Android development)
- Xcode (for iOS development)

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd calorie-tracker-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **iOS Setup** (macOS only)
   ```bash
   cd ios && pod install && cd ..
   ```

4. **Run the application**
   ```bash
   # For Android
   npm run android
   
   # For iOS
   npm run ios
   ```

## Project Structure

```
src/
├── screens/           # All app screens
│   ├── HomeScreen.js
│   ├── BMICalculatorScreen.js
│   ├── CameraScreen.js
│   ├── ManualLogScreen.js
│   ├── BarcodeScannerScreen.js
│   ├── HistoryScreen.js
│   └── ProfileScreen.js
├── database/         # Database management
│   └── DatabaseManager.js
├── styles/           # Theme and styling
│   └── theme.js
└── utils/            # Utility functions
    └── AppInitializer.js
```

## Key Dependencies

- **React Native**: Core framework
- **React Navigation**: Navigation system
- **React Native Paper**: UI components
- **React Native Camera**: Camera and barcode scanning
- **React Native SQLite Storage**: Local database
- **React Native Vector Icons**: Icon library
- **Moment.js**: Date manipulation

## Features in Detail

### BMI Calculation
- Uses standard BMI formula: weight(kg) / height(m)²
- Categorizes results: Underweight, Normal, Overweight, Obese
- Calculates daily calorie needs using Mifflin-St Jeor equation
- Considers gender, age, weight, height, and activity level

### Image Recognition
- Simulates AI-powered food detection
- Provides confidence scores for detected foods
- Estimates nutritional values based on food categories
- Supports common food types with accurate calorie data

### Manual Logging
- Smart food categorization system
- Automatic nutrient estimation based on food types
- Support for various measurement units
- Real-time calorie and nutrient calculations

### Barcode Detection
- Comprehensive barcode format support
- Pre-loaded sample product database
- Automatic nutritional data extraction
- Easy product addition to food logs

## Future Enhancements

- Integration with real food recognition APIs
- Social features and sharing
- Goal setting and tracking
- Exercise logging integration
- Advanced analytics and insights
- Cloud synchronization
- Recipe suggestions based on dietary goals

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue in the repository or contact the development team.
