# learning_management_system
# Clone the project
git clone https://github.com/theprithwisingh/learning_management_system.git

# Move into the directory
cd lms_frontend

# Install dependencies
npm i

# Run the server
npm run dev

# Tailwind CSS Setup
npm install -D tailwindcss postcss autoprefixer

# Create tailwind config file
npx tailwindcss init

# Add file extensions to the tailwind config in tailwind.config.js
echo "module.exports = {
  content: ['./src/**/*.{html,js,jsx,ts,tsx}', './index.html'],
  plugins: [require('daisyui'), require('@tailwindcss/line-clamp')],
};" > tailwind.config.js

# Add Tailwind directives to index.css
echo "@tailwind base;
@tailwind components;
@tailwind utilities;" > ./src/index.css

# Install required dependencies
npm install @reduxjs/toolkit react-redux react-router-dom react-icons react-chartjs-2 chart.js daisyui axios react-hot-toast @tailwindcss/line-clamp

# ESLint Auto Import Sort Setup
npm i -D eslint-plugin-simple-import-sort

# Add the following to .eslint.cjs
echo "module.exports = {
  plugins: ['simple-import-sort'],
  rules: {
    'simple-import-sort/imports': 'error',
  },
};" > .eslint.cjs

# To enable auto import sort on file save in VSCode, enable "Format on Save" in settings
