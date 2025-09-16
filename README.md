# Tailwind-CSS-Tricks-Tips-


1. 🎨 Custom Form Accent Colors
<input type="checkbox" class="accent-pink-500" />
<input type="radio" class="accent-green-500" />


✅ Style checkboxes & radio buttons without custom CSS.

2. 📏 Arbitrary Values with CSS Functions
<p class="text-[min(10vw,10px)]">Responsive text</p>


✅ Use min(), max(), or clamp() directly inside Tailwind.

3. 📂 File Input Styling
<input 
  type="file" 
  class="file:mr-4 file:rounded-lg file:border-0 file:bg-pink-100 file:text-pink-700" 
/>


✅ Style file upload buttons with the file: variant.

4. 🖊️ Custom Text Selection
<p class="selection:bg-green-400 selection:text-white">
  Try selecting this text!
</p>


✅ Change highlight color when selecting text.

5. 📑 Open State Styling with <details>
<details class="open:rotate-90">
  <summary class="cursor-pointer">Toggle me</summary>
  <p>Hidden content...</p>
</details>


✅ Style <details> when expanded using open:.

6. ⌨️ Custom Caret Color
<input 
  type="text" 
  class="caret-pink-500" 
  placeholder="Type here..." 
/>


✅ Change input cursor (caret) color.

7. 🌑 Dark Mode Only Styles
<p class="dark:text-yellow-400">This text glows in dark mode 🌙</p>


✅ Apply styles only when dark mode is enabled.

// tailwind.config.js
module.exports = {
  darkMode: 'class', // or 'media'
}

8. 📱 Container Queries (v3.2+)
<div class="@container">
  <p class="@md:text-xl">Responsive inside parent</p>
</div>


✅ Make elements responsive inside their container, not just viewport.

9. 🎞️ Scrollbar Styling (with plugin)

Install plugin:

npm install tailwind-scrollbar


Enable it:

plugins: [
  require('tailwind-scrollbar'),
],


Usage:

<div class="overflow-y-scroll scrollbar-thin scrollbar-thumb-pink-500 scrollbar-track-gray-200 h-40">
  Long scrollable content...
</div>


✅ Fully customize scrollbars.

10. ⏳ First/Last/Nth Child Styling
<ul>
  <li class="first:text-red-500">First item</li>
  <li class="even:bg-gray-100">Even item</li>
  <li class="last:font-bold">Last item</li>
</ul>


✅ Use first:, last:, even:, and odd: utilities for child elements.
