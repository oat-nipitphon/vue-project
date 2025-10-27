# vue-project
Vue js , Pinia , 

# Tailwind Css 
- npm install -D tailwindcss postcss autoprefixer

- Update Config File tailwind.config.js
  module.exports = {
  content: ['./index.html', './src/**/*.{vue,js,ts}'],
  theme: {
    extend: {},
  },
  plugins: [],
} 

- Update Config File src/assets/main.css
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

- Update File main.js Config use import  assets/main.css


# Tiptap Editor
npm install @tiptap/vue-3 @tiptap/starter-kit
