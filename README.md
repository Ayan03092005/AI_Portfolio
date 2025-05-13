Ayan Chattopadhyay's Portfolio
This is a modern, responsive portfolio website showcasing my skills, projects, and contact information as a 3rd-year BTech CSE student at IEM, graduating in 2027. The site features a clean design, interactive chatbot powered by the Gemini API, and a dark/light theme toggle. It is deployed on Firebase Hosting for fast, reliable access.
Features

Responsive Design: Adapts seamlessly to mobile, tablet, and desktop screens using Tailwind CSS.
Dark/Light Theme Toggle: Switch between themes with persistent state via localStorage.
AI-Powered Chatbot: Ask questions about me, powered by the Gemini API with a centered, animated overlay.
Projects Section: Displays key projects (e.g., E-Commerce Platform, Task Manager) with Pexels thumbnails and hover effects.
Smooth Scrolling: Navigate sections (Home, About, Projects, Contact) with smooth transitions.
Contact Form: Placeholder for collecting user inquiries (backend not implemented).
Animations: Pulse effect for the chat bubble and typing animation for the chatbot.

Technologies Used

HTML5: Structure and content.
Tailwind CSS: Styling and responsive design (via CDN).
JavaScript: Interactivity, theme toggle, and Gemini API integration.
Gemini API: Powers the chatbot for natural, context-aware responses.
Firebase Hosting: Deploys the static site for global access.
Pexels: Provides project thumbnail images.

Setup Instructions
To run the portfolio locally, follow these steps:

Clone the Repository:
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>


Project Structure:

The main file is index.html, located in the root or public directory (depending on Firebase setup).
No additional dependencies are required, as Tailwind CSS is loaded via CDN and images are hosted externally (Pexels, Imgur).


Run Locally:

Open index.html in a browser (e.g., Chrome, Firefox) using a local server to avoid CORS issues:npx http-server

Access at http://localhost:8080.
Alternatively, use VS Code’s Live Server extension.


Configure Gemini API (Optional):

The chatbot uses the Gemini API. To enable it, replace the GEMINI_API_KEY in index.html with your own key:const GEMINI_API_KEY = "your-api-key-here";


Obtain a key from Google AI Studio.
Note: The provided key may have quota limits or expire.

Usage

Dark Theme Toggle: Click the sun/moon icon in the navbar to switch themes.
Chatbot: Click the "Ask anything about me" bubble to open the chatbot. Ask questions about my skills, projects, or interests.
Projects: Hover over project cards to see a scale and shadow effect. Images are sourced from Pexels.
Navigation: Use the navbar links (Home, About, Projects, Contact) for smooth scrolling.
Contact Form: Enter details (currently a placeholder; backend not implemented).

Troubleshooting

Chatbot Not Responding:
Verify the Gemini API key is valid and has quota.
Check the console (F12 > Console) for errors like "Invalid API key" or "Quota exceeded".
Test the API endpoint: https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent.

Images Not Loading:
Ensure Pexels URLs are accessible (e.g., https://images.pexels.com/photos/356056/pexels-photo-356056.jpeg).
Check the Network tab in dev tools for 404 errors.
Replace with alternative Pexels images if needed.

Firebase Deployment Issues:
Confirm index.html is in the public directory specified in firebase.json.
Check CLI output for errors (firebase deploy --debug).
Ensure you have “Firebase Hosting Admin” permissions in the Firebase Console.

Distorted Chatbot Window:
Verify the chat-overlay CSS (flex items-center justify-center, z-index: 50).
Test on multiple screen sizes and clear browser cache.

Contact
Feel free to reach out via GitHub or open an issue in this repository for questions or feedback.

Built with ❤️ by Ayan Chattopadhyay
