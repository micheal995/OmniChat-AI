OmniChat AI, a high-performance customer engagement platform designed to handle multiple simultaneous conversations with ease.
Key Features
Multi-Stream Dashboard: A technical, information-dense workspace that allows agents to monitor and switch between dozens of active customer queries instantly.
AI Auto-Pilot: Powered by Gemini-3-flash, each conversation has a toggleable "AI Pilot." When enabled, the AI automatically analyzes the customer's query and conversation history to provide professional, concise responses in real-time.
Real-time Synchronization: Built on Firebase Firestore, ensuring that all messages and status updates (Active, Pending, Resolved) are synchronized across the platform immediately.
Hardened Security: The application includes a robust suite of Firestore security rules based on zero-trust principles, protecting customer data and preventing "identity poisoning" or unauthorized state changes.
Responsive Technical UI: Designed with a "Mission Control" aesthetic using a dark palette, high-precision typography, and fluid motion transitions for a premium, professional feel.
Technical Implementation
Database: Firestore sub-collections for messages to ensure infinite scalability per chat.
AI Logic: Gemini integration with advanced system instructions to maintain a professional support persona.
Utility: Automatic data seeding on first run so you can see the multi-conversation handling in action immediately.
You can now start managing customer queries, toggle the AI Pilot for automated support, and resolve issues directly from the dashboard.
# GEMINI_API_KEY: Required for Gemini AI API calls.
# AI Studio automatically injects this at runtime from user secrets.
# Users configure this via the Secrets panel in the AI Studio UI.
GEMINI_API_KEY="MY_GEMINI_API_KEY"

# APP_URL: The URL where this applet is hosted.
# AI Studio automatically injects this at runtime with the Cloud Run service URL.
# Used for self-referential links, OAuth callbacks, and API endpoints.
APP_URL="MY_APP_URL"
