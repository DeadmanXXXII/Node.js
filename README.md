# Node.js
Here's an extensive and detailed list of Node.js CLI commands:

### **Node.js CLI Commands**

#### **1. Node.js Version Management**

- **Check Node.js version:**
  ```bash
  node -v
  ```

- **Check npm version:**
  ```bash
  npm -v
  ```

- **Update Node.js (using nvm - Node Version Manager):**
  ```bash
  nvm install node # Install latest version
  nvm install <version> # Install specific version
  nvm use <version> # Switch to specific version
  ```

- **List installed Node.js versions (using nvm):**
  ```bash
  nvm ls
  ```

- **List available Node.js versions (using nvm):**
  ```bash
  nvm ls-remote
  ```

#### **2. Node.js Script Execution**

- **Run a Node.js script:**
  ```bash
  node script.js
  ```

- **Run a script with additional arguments:**
  ```bash
  node script.js arg1 arg2
  ```

- **Run a script with environment variables:**
  ```bash
  NODE_ENV=production node script.js
  ```

- **Run Node.js in REPL (Read-Eval-Print Loop) mode:**
  ```bash
  node
  ```

- **Run Node.js with debugging:**
  ```bash
  node --inspect script.js
  ```

#### **3. npm (Node Package Manager) Commands**

- **Initialize a new Node.js project:**
  ```bash
  npm init
  ```

- **Initialize a new Node.js project with default settings:**
  ```bash
  npm init -y
  ```

- **Install a package locally:**
  ```bash
  npm install package-name
  ```

- **Install a package globally:**
  ```bash
  npm install -g package-name
  ```

- **Uninstall a package:**
  ```bash
  npm uninstall package-name
  ```

- **List installed packages:**
  ```bash
  npm list
  ```

- **Update all packages to their latest versions:**
  ```bash
  npm update
  ```

- **Check for outdated packages:**
  ```bash
  npm outdated
  ```

- **Check for security vulnerabilities in installed packages:**
  ```bash
  npm audit
  ```

- **Audit and fix vulnerabilities:**
  ```bash
  npm audit fix
  ```

- **Generate a package-lock.json file:**
  ```bash
  npm install
  ```

- **Run scripts defined in package.json:**
  ```bash
  npm run script-name
  ```

- **View details of a specific package:**
  ```bash
  npm view package-name
  ```

#### **4. npx (Node Package Runner)**

- **Run a package without installing it:**
  ```bash
  npx package-name
  ```

- **Run a specific version of a package:**
  ```bash
  npx package-name@version
  ```

- **Run a command from a package:**
  ```bash
  npx package-name command
  ```

#### **5. Node.js Advanced Commands**

- **Run Node.js with V8 Inspector:**
  ```bash
  node --inspect-brk script.js
  ```

- **Run Node.js with Trace:**
  ```bash
  node --trace-warnings script.js
  ```

- **Run Node.js with Profiling:**
  ```bash
  node --prof script.js
  ```

- **Generate a heap snapshot:**
  ```bash
  node --inspect script.js
  ```

#### **6. Node.js Debugging**

- **Start debugging with the `inspect` flag:**
  ```bash
  node --inspect script.js
  ```

- **Start debugging with the `inspect-brk` flag (breaks before user code runs):**
  ```bash
  node --inspect-brk script.js
  ```

- **Debug in Chrome DevTools:**
  Open `chrome://inspect` in Chrome and click "Open dedicated DevTools for Node".

- **Debug with Visual Studio Code:**
  Configure `.vscode/launch.json` and use the "Run and Debug" pane.

#### **7. Node.js Performance Monitoring**

- **Measure performance with the built-in profiler:**
  ```bash
  node --prof script.js
  ```

- **Analyze the generated V8 log:**
  ```bash
  node --prof-process isolate-0xnnnnnnnnnnnn-v8.log
  ```

#### **8. Node.js Package Development**

- **Create a new package template:**
  ```bash
  npm init
  ```

- **Link a local package for development:**
  ```bash
  npm link
  ```

- **Publish a package to npm registry:**
  ```bash
  npm publish
  ```

- **View package publish history:**
  ```bash
  npm view package-name
  ```

- **Access package information from the npm registry:**
  ```bash
  npm info package-name
  ```

#### **9. Node.js Testing**

- **Run tests defined in package.json (e.g., with Mocha):**
  ```bash
  npm test
  ```

- **Run tests with a specific framework (e.g., Jest):**
  ```bash
  npx jest
  ```

- **Run tests with a specific environment variable:**
  ```bash
  TEST_ENV=production npx mocha
  ```

#### **10. Node.js Code Quality and Linting**

- **Run ESLint for linting JavaScript code:**
  ```bash
  npx eslint filename.js
  ```

- **Fix linting issues automatically:**
  ```bash
  npx eslint filename.js --fix
  ```

- **Check code formatting with Prettier:**
  ```bash
  npx prettier --check filename.js
  ```

- **Format code with Prettier:**
  ```bash
  npx prettier --write filename.js
  ```

#### **11. Node.js Environment Management**

- **Set environment variables temporarily:**
  ```bash
  ENV_VAR=value node script.js
  ```

- **Use `.env` files with `dotenv` package:**
  ```bash
  npm install dotenv
  ```

  In `script.js`:
  ```javascript
  require('dotenv').config();
  console.log(process.env.ENV_VAR);
  ```

### **Summary**

This comprehensive list includes fundamental and advanced Node.js CLI commands, package management, debugging, performance monitoring, testing, and code quality tools. It covers common practices for managing Node.js environments, developing and testing applications, and ensuring code quality.
