🧑💻 Development
----------------

### Available Scripts

**CommandDescription**npm run start:devStart dev server with live reloadnpm run buildCompile TypeScript to productionnpm run ts.checkType-check without emitting filesnpm startRun production build

### Workflow

1.  bashCopynpm run start:devServer runs at http://localhost:3000
    
2.  Make changes in src/ directory
    
3.  Commit changes (automatically triggers pre-commit validation)
    

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

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   graph LR    A[Commit Attempt] --> B{Type Check}    B -->|Pass| C[Production Build]    C --> D[Add Built Files]    D --> E[Commit Complete]    B -->|Fail| F[Abort Commit]   `

⚙️ Environment Variables
------------------------

**VariableDefaultDescription**PORT3000Server port

📁 Project Structure
--------------------

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   .  ├── src/            # TypeScript source  │   └── index.ts    # Entry point  ├── dist/           # Compiled JS (auto-generated)  ├── .env            # Environment variables  ├── tsconfig.json   # TypeScript config  └── vercel.json     # Vercel configuration   `

🤝 Contributing
---------------

1.  Fork the project
    
2.  Create feature branch (git checkout -b feature/AmazingFeature)
    
3.  Commit changes (git commit -m 'Add AmazingFeature')
    
4.  Push branch (git push origin feature/AmazingFeature)
    
5.  Open Pull Request
    

📄 License
----------

Distributed under the ISC License. See LICENSE for details.

Made with ❤️ by \[Your Name\] | Deployed on