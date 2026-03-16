# Aura Travel

Aura Travel is a modern, full-stack Next.js web application designed using Google's Antigravity to help users find the best economy flight tickets optimized for cost and travel time. It features a stunning, dynamic user interface built with strict Vanilla CSS (no Tailwind) and a simulated backend API for flight searching and realistic secure checkout.

## Features

- **Lightning Fast Search**: Intelligent mock API that generates and sorts flights to find the absolute best options combining lowest price and shortest duration.
- **Dynamic Visuals**: Stunning glassmorphism UI, vibrant color palettes, and micro-animations to enhance user experience.
- **Comparative Results**: Automatically badges the "Fastest" and "Best Value" flights for quick decision-making.
- **Secure Mock Checkout**: A seamless redirect flow to a simulated secure payment page.
- **Responsive Design**: Built to look great on both desktop and mobile devices using modern CSS layouts.
- **Next.js App Router**: Utilizes the latest Next.js 14/15 routing paradigms including Server and Client components.

## Tech Stack

- **Framework**: Next.js (React)
- **Language**: TypeScript
- **Styling**: Vanilla CSS (CSS Modules / Global Styles)
- **Backend**: Next.js API Routes (Mock Data Generation)

## Getting Started

Follow these instructions to get the project up and running on your local machine.

### Prerequisites

- Node.js (v18 or higher recommended)
- npm (Node Package Manager)

### Installation

1. Clone the repository or download the source code:
   ```bash
   git clone <repository-url>
   cd agentic_ai
   ```

2. Install the application dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

## Project Structure

- `/app/layout.tsx`: The root Next.js layout containing the navigation bar and global metadata.
- `/app/page.tsx`: The main landing page featuring the hero section and flight search form.
- `/app/search/page.tsx`: The search results page that queries the API and displays the flight list.
- `/app/booking/page.tsx`: The checkout experience displaying order summary and a mock payment form.
- `/app/api/flights/route.ts`: The Next.js API route responsible for generating and sorting the simulated flight data.
- `/components/`: Reusable React components (`FlightSearchForm`, `FlightList`, `FlightCard`) and their associated Vanilla CSS files.
- `/app/globals.css`: The core design system containing CSS variables, utility classes, and global resets.

## Future Enhancements
- Integration with live flight providers (e.g., Amadeus or Skyscanner API) for real-time data.
- User authentication and persistent trip saving.
- Integration with Stripe for actual payment processing.
