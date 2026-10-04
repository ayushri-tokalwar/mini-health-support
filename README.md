# Mini Health Support 🏥

A modern, responsive healthcare NGO web platform built with **React 19**, **Vite 8**, **Tailwind CSS v4**, and **GSAP**. This application connects patients in need with essential healthcare support, manages volunteer registrations, and provides an AI-powered healthcare assistant (**HealthBot**) for real-time guidance.

---

## ✨ Features

- **🏥 Patient Support Portal**:
  - Request medical assistance, home care, patient transport, medicine delivery, and psychological counseling.
  - Interactive multi-step form with validation and smooth GSAP animations.

- **🤝 Volunteer Registration**:
  - Onboarding workflow for doctors, nurses, drivers, counselors, and community volunteers.
  - Role-based registration with availability selection and district coverage.

- **🤖 AI Healthcare Assistant ("HealthBot")**:
  - Integrated intelligent chatbot powered by the **SambaNova Cloud API** (`gpt-oss-120b`).
  - Provides reliable NGO service information, general wellness FAQs, and immediate emergency redirection (108 / 112).
  - Voice recognition and speech synthesis support for enhanced accessibility.

- **🎨 Modern Aesthetic & Animation**:
  - Styled with Tailwind CSS v4.
  - Fluid micro-interactions powered by GSAP & ScrollTrigger.
  - Fully responsive across desktop, tablet, and mobile devices.

---

## 🛠️ Tech Stack

- **Frontend Framework**: [React 19](https://react.dev/)
- **Build Tool**: [Vite 8](https://vitejs.dev/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Animations**: [GSAP (GreenSock)](https://greensock.com/gsap/) & ScrollTrigger
- **Routing**: [React Router v7](https://reactrouter.com/)
- **Form Management**: [React Hook Form](https://react-hook-form.com/)
- **AI Integration**: [SambaNova Cloud API](https://sambanova.ai/)

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed on your system:
- [Node.js](https://nodejs.org/) (v18.0.0 or higher, v20+ recommended)
- [npm](https://www.npmjs.com/) (v9.0.0 or higher)

### 1. Clone the Repository

```bash
git clone https://github.com/ayushri-tokalwar/mini-health-support.git
cd mini-health-support
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory (you can copy `.env.example`):

```bash
cp .env.example .env
```

Add your SambaNova API key to enable the AI HealthBot:

```env
VITE_SAMBANOVA_API_KEY=your_sambanova_api_key_here
VITE_SAMBANOVA_MODEL=gpt-oss-120b
```

> **Note**: You can obtain a free API key at [SambaNova Cloud](https://cloud.sambanova.ai/).

### 4. Run the Development Server

```bash
npm run dev
```

Open your browser and navigate to:
```
http://localhost:5173/
```

---

## 📜 Available Scripts

| Command | Description |
| :--- | :--- |
| `npm run dev` | Starts Vite local development server with Hot Module Replacement (HMR) |
| `npm run build` | Builds optimized production bundle in the `dist/` directory |
| `npm run preview` | Locally previews the production build |
| `npm run lint` | Runs ESLint to check for code quality and style issues |
| `npm run deploy` | Deploys the built application to GitHub Pages |

---

## 📁 Project Structure

```text
mini-health-support/
├── public/                 # Static assets
├── src/
│   ├── assets/             # Images and design assets
│   ├── component/          # Core application components
│   │   ├── Aichatbot.jsx                # AI HealthBot assistant component
│   │   ├── Herosection.jsx              # Landing hero banner & stats
│   │   ├── PatientSupportPage.jsx       # Patient assistance request portal
│   │   ├── Volunteerregistrationform.jsx# Volunteer registration portal
│   │   └── Voiceservice.js              # Voice synthesis & speech recognition
│   ├── App.jsx             # Main layout, router & navigation
│   ├── main.jsx            # Application entry point
│   ├── index.css           # Global Tailwind CSS styles
│   └── App.css             # Component-specific styles
├── .env.example            # Environment variables template
├── eslint.config.js        # ESLint configuration
├── package.json            # Project dependencies and npm scripts
├── postcss.config.mjs      # PostCSS configuration for Tailwind
└── vite.config.js          # Vite build and base path configuration
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
