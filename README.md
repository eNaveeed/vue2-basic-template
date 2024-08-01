# Vue 2 Basic Template

## Project Setup

Follow these steps to set up your Vue 2 project with TailwindCSS:

### Step 1: Create a Project Folder
1. Create an empty folder for your project.

### Step 2: Initialize Vue Project
2. Open your terminal and run:
    ```bash
    vue create .
    ```

### Step 3: Install TailwindCSS
3. Install TailwindCSS as a development dependency:
    ```bash
    npm install -D tailwindcss
    ```

### Step 4: Initialize TailwindCSS
4. Create the TailwindCSS configuration file:
    ```bash
    npx tailwindcss init
    ```

### Step 5: Configure TailwindCSS
5. In `tailwind.config.js`, replace the `content` array with:
    ```js
    content: ["./src/**/*.{html,js}"],
    ```

### Step 6: Create Tailwind Input CSS
6. Create a file named `src/input.css` and add the following content:
    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

### Step 7: Import Tailwind Output CSS
7. In `App.vue`, under the `<script>` tag, import the output CSS file:
    ```js
    import './output.css'
    ```

### Step 8: Start Development Server
8. In Git Bash or your terminal, spin up the local server:
    ```bash
    npm run serve
    ```

### Step 9: Activate Tailwind Watcher
9. In another terminal window, start the TailwindCSS watcher:
    ```bash
    npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
    ```
