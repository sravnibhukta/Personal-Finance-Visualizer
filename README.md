# 💰 Personal Finance Visualizer

A comprehensive full-stack web application for tracking personal finances with transaction management, categorization, budgeting, and beautiful data visualizations.

![image](https://github.com/user-attachments/assets/dbb514cf-6a0a-44cb-a3f6-66c31c20481d)

![image](https://github.com/user-attachments/assets/42f524b0-08f2-44bc-a260-8a8a0c763d7d)

![image](https://github.com/user-attachments/assets/0c107bb0-a8dc-453e-81c7-8a5d9c277c9a)

![image](https://github.com/user-attachments/assets/27365eb6-5cdf-4234-93b3-8bde4a323b1b)





## ✨ Features

### 📊 Transaction Management
- Add, edit, and delete financial transactions
- Categorize expenses with custom categories
- Real-time transaction tracking
- Beautiful transaction table with sorting and filtering

### 📈 Data Visualization
- Monthly expense trends with interactive charts
- Category breakdown with pie charts
- Spending analytics and insights
- Colorful visual indicators

### 🎯 Budget Management
- Create monthly and yearly budgets by category
- Real-time budget vs actual spending tracking
- Visual progress indicators with color-coded alerts
- Over-budget notifications and warnings
- Comprehensive budget management interface

### 🎨 Beautiful UI
- Modern, responsive design with Tailwind CSS
- Emoji-enhanced interface for better user experience
- Dark/light mode support
- Mobile-friendly responsive layout
- Smooth animations and transitions

## 🚀 Tech Stack

### Frontend
- **React 18** with TypeScript
- **Tailwind CSS** for styling
- **Radix UI** + **shadcn/ui** for components
- **TanStack Query** for state management
- **Wouter** for routing
- **React Hook Form** + **Zod** for form validation
- **Recharts** for data visualization

### Backend
- **Node.js** with **Express.js**
- **TypeScript** with ES modules
- **Drizzle ORM** for database operations
- **Zod** for data validation
- **In-memory storage** for demo purposes

### Development Tools
- **Vite** for frontend development
- **ESBuild** for backend bundling
- **TypeScript** for type safety
- **Replit** for development environment

## 🏁 Getting Started

### Prerequisites
- Node.js 18 or higher
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd personal-finance-visualizer
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5000`

## 📖 Usage

### Adding Transactions
1. Navigate to the Dashboard or Transactions page
2. Click the "Add Transaction" button
3. Fill in the transaction details (description, amount, category, date)
4. Click "Add Transaction" to save

### Managing Categories
- The app comes with pre-configured categories (Food & Dining, Shopping, Transportation, etc.)
- Each category has a unique color and emoji for easy identification

### Setting Up Budgets
1. Go to the Budgets page
2. Click "Add Budget" 
3. Select a category, set the budget amount, and choose the period (Monthly/Yearly)
4. Track your progress with visual indicators

### Viewing Analytics
- Dashboard provides an overview of your financial health
- Monthly charts show spending trends over time
- Category breakdowns help identify spending patterns
- Budget status cards show real-time progress

## 🗂️ Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── lib/            # Utility functions
│   │   └── App.tsx         # Main app component
├── server/                 # Backend Express application
│   ├── index.ts           # Express server setup
│   ├── routes.ts          # API route definitions
│   ├── storage.ts         # Data storage interface
│   └── vite.ts            # Vite integration
├── shared/                 # Shared types and schemas
│   └── schema.ts          # Database schemas and types
└── README.md              # This file
```

## 🔧 API Endpoints

### Transactions
- `GET /api/transactions` - Get all transactions
- `POST /api/transactions` - Create a new transaction
- `PUT /api/transactions/:id` - Update a transaction
- `DELETE /api/transactions/:id` - Delete a transaction

### Categories
- `GET /api/categories` - Get all categories

### Budgets
- `GET /api/budgets` - Get all budgets
- `POST /api/budgets` - Create a new budget
- `PUT /api/budgets/:id` - Update a budget
- `DELETE /api/budgets/:id` - Delete a budget
- `GET /api/budgets-progress` - Get budget progress data

### Analytics
- `GET /api/analytics/summary` - Get financial summary
- `GET /api/analytics/monthly` - Get monthly expense data
- `GET /api/analytics/categories` - Get category breakdown

## 🎨 Customization

### Adding New Categories
Edit the `seedCategories()` method in `server/storage.ts` to add new expense categories with custom colors and emojis.

### Styling
The app uses Tailwind CSS with custom color schemes. Modify `client/src/index.css` to customize the color palette.

### Adding Features
1. Update the database schema in `shared/schema.ts`
2. Add new storage methods in `server/storage.ts`
3. Create API endpoints in `server/routes.ts`
4. Build frontend components in `client/src/components/`

## 🚀 Deployment

### Quick Deploy to Vercel

#### Option 1: Using Vercel CLI
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts to deploy

#### Option 2: Using GitHub Integration
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Vercel will automatically deploy your app

#### Option 3: Manual Upload
1. Build the project: `npm run build`
2. Upload the `dist` folder to Vercel
3. Configure as a static site

### Deployment Configuration
The project includes a `vercel.json` configuration file optimized for deployment:
- Frontend assets are served from `dist/public`
- API routes are handled by serverless functions
- Both development and production environments are supported

### Environment Variables
For production deployment, you may need to set:
- `NODE_ENV=production`
- Any database connection strings (if using a real database)

### Live Demo
Once deployed, your app will be available at: `https://your-app-name.vercel.app`

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

If you encounter any issues or have questions, please open an issue in the GitHub repository.

---

**Built with ❤️ using React, Express, and modern web technologies**
