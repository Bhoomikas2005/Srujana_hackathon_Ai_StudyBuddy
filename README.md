# AI Study Buddy - React Frontend

A comprehensive React.js frontend for the AI Study Buddy platform featuring authentication, study tracking, AI-powered quizzes, chatbot companion, and gamification elements.

## 🚀 Features

### 🔐 Authentication System
- **Login & Registration**: Beautiful, responsive forms with validation
- **JWT Token Management**: Secure token storage and automatic refresh
- **Protected Routes**: Route protection with redirect to login
- **User Profile Management**: Update profile and change password

### 📊 Dashboard
- **XP & Level Display**: Real-time XP and level progression
- **Badges & Achievements**: Visual badge collection with animations
- **Study Streaks**: Track daily study consistency
- **Quick Actions**: Easy access to all platform features
- **Progress Overview**: Visual progress indicators and statistics

### ⏱️ Study Session Timer
- **Webcam Integration**: Real-time webcam feed for focus monitoring
- **AI Focus Detection**: Simulated focus tracking with motivational messages
- **Session Management**: Start, pause, and end study sessions
- **Topic Tracking**: Add and manage study topics
- **Focus Score**: Real-time focus score calculation
- **Session Notes**: Add notes during study sessions

### 📚 AI Study Plan & Syllabus
- **Course Selection**: Choose from multiple courses (1st PU, 2nd PU, degrees)
- **Subject Management**: Organized by subjects and chapters
- **Topic Breakdown**: Detailed topic lists with difficulty levels
- **Video Integration**: Embedded video links for each chapter
- **Progress Tracking**: Mark chapters as complete
- **AI Study Tips**: Personalized study recommendations
- **Search Functionality**: Search across topics and subjects

### 🧠 AI Quiz Generator
- **Custom Quiz Creation**: Generate quizzes based on selected topics
- **Difficulty Levels**: Easy, medium, and hard difficulty options
- **Real-time Timer**: Timed quiz sessions with countdown
- **Interactive Questions**: Multiple choice with immediate feedback
- **Detailed Results**: Comprehensive score breakdown and explanations
- **XP Rewards**: Earn XP based on performance
- **Quiz History**: Track past quiz attempts and scores

### 💬 AI Chatbot Companion
- **Intelligent Conversations**: Context-aware AI responses
- **Topic-specific Help**: Focused assistance based on study topics
- **Chat History**: Persistent conversation history
- **Message Rating**: Rate AI responses for continuous improvement
- **Study Tips Generation**: AI-generated study tips and advice
- **Quick Questions**: Pre-defined helpful questions

### 🏆 Gamification System
- **XP System**: Earn experience points for all activities
- **Level Progression**: Automatic level advancement
- **Badge Collection**: Unlock achievements and badges
- **Leaderboard**: Compete with other students
- **Streak Tracking**: Daily study streak maintenance
- **Progress Milestones**: Visual milestone tracking

## 🛠️ Tech Stack

- **Framework**: React 18 with Hooks
- **Routing**: React Router v6
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **HTTP Client**: Axios
- **Webcam**: React Webcam
- **Notifications**: React Hot Toast
- **Effects**: React Confetti
- **Build Tool**: Vite
- **State Management**: Context API + useReducer

## 📁 Project Structure

```
src/
├── components/           # Reusable UI components
│   ├── Layout.jsx       # Main layout with sidebar
│   ├── ProtectedRoute.jsx # Route protection
│   └── StudyTimer.jsx   # Study timer component
├── contexts/            # React Context providers
│   ├── AuthContext.jsx  # Authentication state
│   └── StudyContext.jsx # Study session state
├── pages/               # Page components
│   ├── Login.jsx        # Login page
│   ├── Register.jsx     # Registration page
│   ├── Dashboard.jsx    # Main dashboard
│   ├── StudyPlan.jsx    # Study plan and syllabus
│   ├── Quiz.jsx         # Quiz generator and taking
│   ├── Chat.jsx         # AI chatbot interface
│   ├── Leaderboard.jsx  # Leaderboard and rankings
│   └── Achievements.jsx # Badges and achievements
├── utils/               # Utility functions
│   └── api.js          # API client and endpoints
├── App.jsx             # Main App component
├── main.jsx            # App entry point
└── index.css           # Global styles
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Running backend API server

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd ai-study-buddy-frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   ```bash
   cp env.example .env
   ```
   
   Update the `.env` file:
   ```env
   VITE_API_URL=http://localhost:5000/api
   VITE_APP_NAME=AI Study Buddy
   VITE_APP_VERSION=1.0.0
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

## 🎨 UI/UX Features

### Design System
- **Color Palette**: Primary (blue), secondary (green), accent (yellow)
- **Typography**: Clean, readable fonts with proper hierarchy
- **Spacing**: Consistent spacing using Tailwind's scale
- **Responsive**: Mobile-first responsive design
- **Animations**: Smooth transitions and micro-interactions

### Accessibility
- **Keyboard Navigation**: Full keyboard support
- **Screen Readers**: Proper ARIA labels and semantic HTML
- **Color Contrast**: WCAG compliant color combinations
- **Focus Indicators**: Clear focus states for all interactive elements

### Performance
- **Code Splitting**: Automatic route-based code splitting
- **Lazy Loading**: Lazy load heavy components
- **Optimized Images**: Proper image optimization
- **Bundle Analysis**: Built-in bundle size analysis

## 📱 Responsive Design

The application is fully responsive and works seamlessly across:
- **Desktop**: Full-featured experience with sidebar navigation
- **Tablet**: Adapted layout with collapsible sidebar
- **Mobile**: Touch-optimized interface with bottom navigation

## 🔧 Configuration

### API Integration
All API calls are centralized in `src/utils/api.js` with:
- Automatic token injection
- Request/response interceptors
- Error handling
- Base URL configuration

### Styling
- **Tailwind CSS**: Utility-first CSS framework
- **Custom Components**: Reusable component classes
- **Theme Configuration**: Customizable color schemes
- **Dark Mode Ready**: Easy dark mode implementation

## 🧪 Development

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Code Structure
- **Functional Components**: All components use React hooks
- **Custom Hooks**: Reusable logic in custom hooks
- **Context API**: Global state management
- **Error Boundaries**: Proper error handling

## 🔒 Security Features

- **JWT Token Management**: Secure token storage and refresh
- **Route Protection**: Authentication-based route access
- **Input Validation**: Client-side form validation
- **XSS Prevention**: Proper data sanitization
- **CSRF Protection**: Token-based request validation

## 🎯 Key Components

### Dashboard
- Real-time statistics display
- Quick action buttons
- Recent achievements showcase
- Study streak visualization
- Leaderboard preview

### Study Timer
- Webcam integration for focus monitoring
- Real-time timer with pause/resume
- Focus score calculation
- Motivational messages
- Session statistics

### Quiz System
- AI-generated questions
- Multiple difficulty levels
- Real-time scoring
- Detailed explanations
- Performance analytics

### Chat Interface
- Real-time AI responses
- Message history
- Rating system
- Study tips generation
- Topic-specific assistance

## 🚀 Deployment

### Production Build
```bash
npm run build
```

### Environment Variables
Set the following environment variables for production:
- `VITE_API_URL`: Production API URL
- `VITE_APP_NAME`: Application name
- `VITE_APP_VERSION`: Version number

### Hosting Options
- **Vercel**: Zero-config deployment
- **Netlify**: Continuous deployment from Git
- **AWS S3 + CloudFront**: Scalable static hosting
- **Firebase Hosting**: Google's hosting solution

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- React team for the amazing framework
- Tailwind CSS for the utility-first approach
- Framer Motion for smooth animations
- Lucide for beautiful icons
- OpenAI for AI capabilities

---

Built with ❤️ for better learning experiences