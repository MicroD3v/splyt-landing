# Spylt 🥤

A high-performance landing page for a caffeinated protein milk brand. This project focuses on modern web layouts mixed with fluid, scroll-driven motion design and interactive product scaling.

<p align="center">
  <img src="public/videos/spylt-intro.gif" alt="Spylt Animation Preview" width="800px"/>
</p>





🎯 **[Check out the live website here](https://splyt-landing-five.vercel.app/)**


---

## ✨ Key Motion Features

*   **Assembling Intro**: A coordinated canvas assembly on page load that brings separate layout elements together seamlessly.
*   **Dynamic Product Routing**: Specialized product assets that track down the screen and shift depth based on user scroll position.
*   **Scroll-Bound Timelines**: Layout transformations and typography fades mapped smoothly to the viewport scroll bar.
*   **Responsive Breakpoints**: Custom media scaling ensuring complex timelines preserve layout alignment on mobile views.

## 🛠️ The Stack

*   **Core Framework**: React 19 & Vite 8
*   **Styling Engine**: Tailwind CSS v4
*   **Animation Engine**: GSAP (GreenSock Animation Platform)
*   **React Integration**: `@gsap/react` (leveraging the official `useGSAP` hook for automated animation lifecycles)
*   **Responsive Control**: `react-responsive`

## ⚙️ Local Development Setup

Get the code running on your machine locally in under two minutes:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/MicroD3v/splyt-landing.git
   ```

2. **Navigate into the directory:**

   ```bash
   cd splyt-landing
   ```

3. **Install dependencies:**

   ```bash
   npm install
   ```

4. **Launch the local Vite server:**

   ```bash
   npm run dev
   ```


## 🧠 Technical Takeaways & Performance

Mixing standard web layouts with continuous scroll-tied timelines provided excellent insights into optimization:
*   **Safe Lifecycle Handling**: Implemented the official `@gsap/react` library's `useGSAP()` hook. This ensures all active timelines automatically revert and clean up when components unmount, eliminating layout shifts and memory leaks.
*   **60 FPS Rendering**: Prioritized hardware-accelerated animations by targeting CSS transforms (`x`, `y`, `scale`) rather than document layout properties like `top` or `left` to keep screen painting smooth.
*   **Vite 8 Build Speeds**: Leveraged the dedicated `@tailwindcss/vite` plugin for fast hot-module replacement (HMR), keeping timeline state stable while testing motion behaviors.


