# Onlooks - Student Dropout Prediction System

A modern web application for predicting student dropout risk using machine learning. Built with Next.js, TypeScript, and TailwindCSS.

![Next.js](https://img.shields.io/badge/Next.js-14.2-black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4-38bdf8)
![License](https://img.shields.io/badge/license-MIT-green)

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Environment Variables](#environment-variables)
- [Available Scripts](#available-scripts)
- [Testing](#testing)
- [Contributing](#contributing)

## ✨ Features

- **🔐 Authentication System**: Secure JWT-based login and registration
- **📊 Dashboard**: Visual analytics with interactive charts for attendance and student metrics
- **🎯 Dropout Predictions**: AI-powered student dropout risk assessment
- **📁 File Upload**: Batch upload student data via CSV files
- **📈 Prediction Analytics**: Detailed prediction summaries and insights
- **🌓 Dark Mode**: Built-in theme switching support
- **📱 Responsive Design**: Mobile-first, responsive UI components
- **♿ Accessibility**: WCAG compliant with Radix UI primitives

## 🛠️ Tech Stack

### Frontend
- **Framework**: [Next.js 14](https://nextjs.org/) (App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: [TailwindCSS](https://tailwindcss.com/)
- **UI Components**: [Radix UI](https://www.radix-ui.com/) + [shadcn/ui](https://ui.shadcn.com/)
- **Charts**: [Recharts](https://recharts.org/) & [Chart.js](https://www.chartjs.org/)
- **Form Handling**: [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)
- **Icons**: [Lucide React](https://lucide.dev/)

### Testing
- **Unit Tests**: [Jest](https://jestjs.io/) & [Vitest](https://vitest.dev/)
- **Component Tests**: [React Testing Library](https://testing-library.com/react)
- **Test Environment**: jsdom & happy-dom

## 🚀 Getting Started

### Prerequisites

- Node.js 18.x or higher
- npm, yarn, pnpm, or bun package manager
- Access to the backend API

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd DropLookout-UI
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   # or
   bun install
   ```

3. **Set up environment variables**
   
   Copy the example environment file and configure it:
   ```bash
   cp .env.example .env.local
   ```
   
   Update `.env.local` with your settings:
   ```env
   NEXT_PUBLIC_API_URL=http://your-api-url:8000
   NODE_ENV=development
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📁 Project Structure

```
DropLookout-UI/
├── app/                      # Next.js App Router pages
│   ├── dashboard/           # Dashboard page
│   ├── login/              # Authentication pages
│   ├── register/
│   ├── predictions/        # Prediction results
│   ├── upload/             # File upload page
│   └── layout.tsx          # Root layout
├── components/              # React components
│   ├── dashboard/          # Dashboard-specific components
│   ├── layout/             # Layout components (navbar, etc.)
│   ├── predictions/        # Prediction components
│   └── ui/                 # Reusable UI components (shadcn/ui)
├── config/                  # App configuration
├── context/                 # React Context providers
├── hooks/                   # Custom React hooks
│   ├── useApi.ts           # API hook
│   └── __tests__/          # Hook tests
├── lib/                     # Utility functions
├── public/                  # Static assets
└── styles/                  # Global styles
```

## 🔧 Environment Variables

| Variable | Description | Default | Required |
|----------|-------------|---------|----------|
| `NEXT_PUBLIC_API_URL` | Backend API URL | See `.env.example` | Yes (Production) |
| `NODE_ENV` | Environment mode | `development` | No |

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server on port 3000 |
| `npm run build` | Build production bundle |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint for code quality |
| `npm test` | Run test suite |

## 🧪 Testing

The project uses both Jest and Vitest for testing:

### Run Tests
```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage
```

### Test Structure
- Component tests: `components/**/__tests__/*.test.tsx`
- Hook tests: `hooks/__tests__/*.test.ts`
- Test setup: `jest.setup.js` and `vitest.setup.ts`

## 🎨 Key Features Explained

### Authentication Flow
- JWT-based authentication with token storage
- Automatic token validation and expiry checking
- Protected routes with authentication guards

### Dashboard
- Real-time student metrics visualization
- Attendance tracking with interactive charts
- Quick access to prediction summaries

### Predictions
- Upload student data via CSV files
- Batch prediction processing
- Individual prediction cards with risk levels
- Comprehensive prediction summaries

### File Upload
- CSV template download
- Drag-and-drop file upload
- Data validation before submission

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Code Style

This project follows:
- ESLint configuration for code quality
- TypeScript strict mode
- Prettier for code formatting (if configured)

## 📄 License

This project is private and proprietary.

## 👥 Authors

- Your Team Name

## 🙏 Acknowledgments

- [shadcn/ui](https://ui.shadcn.com/) for the beautiful component library
- [Radix UI](https://www.radix-ui.com/) for accessible primitives
- [Vercel](https://vercel.com/) for Next.js

## 📞 Support

For support, please contact your development team or open an issue in the repository.

---

**Built with ❤️ using Next.js**

