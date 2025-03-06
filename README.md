# Node.js + Express + TypeScript Boilerplate for Vercel 🚀

A starter template for building and deploying Express applications with TypeScript on Vercel, featuring pre-commit hooks and seamless deployment workflows.

## ✨ Features

- **TypeScript First**  
  Full TypeScript support with strict type checking
- **Vercel Optimized**  
  Ready for serverless deployment out-of-the-box
- **Git Hooks**  
  Husky pre-commit validation
- **Dev/Prod Parity**  
  Identical environment in development and production
- **Dotenv Support**  
  Environment variables management

## 📋 Prerequisites

- Node.js 18+
- npm 9+
- Vercel account
- Basic understanding of TypeScript

## 🛠️ Installation

1. Clone repository:
   ```bash
   git clone https://github.com/your-username/node-express-typescript-on-vercel.git
   cd node-express-typescript-on-vercel

2. Install dependencies:
   ```bash
   npm install

3. Set up environment variables:
   ```bash
   cp .env.example .env

🧑💻 Development
----------------

### Available Scripts

| Command	 | Description |
| ----------- | ----------- |
| `npm run start:dev` | Start dev server with live reload   |
| `npm run build` | Compile TypeScript to production   |
| `npm run ts.check` | Type-check without emitting files   |
| `npm start` | Run production build   |

### Workflow

1.  Start development server:
   ```bash
      npm run start:dev
   ```
   Server runs at `http://localhost:3000`

3.  Make changes in `src/` directory
    
4.  Commit changes (automatically triggers pre-commit validation)
    

☁️ Vercel Deployment
--------------------

1.  Push code to your Git repository
    
2.  [Import Project](https://vercel.com/new) in Vercel dashboard
    
3.  Configure settings:
    
    *   **Build Command:** npm run build
        
    *   **Output Directory:** dist
        
    *   Add environment variables from .env
        
4.  Deploy! 🚀
    

🔒 Pre-Commit Validation
------------------------
 ```bash
  graph LR
    A[Commit Attempt] --> B{Type Check}
    B -->|Pass| C[Production Build]
    C --> D[Add Built Files]
    D --> E[Commit Complete]
    B -->|Fail| F[Abort Commit]

