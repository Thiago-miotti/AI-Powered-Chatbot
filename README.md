# AI-Powered Chatbot

A fully functional AI-powered chatbot built with a modern full-stack architecture, featuring real-time conversations, markdown support, and a polished user interface.

## 🚀 Features

- **AI-Powered Responses**: Integrated with OpenAI API for intelligent conversation
- **Real-time Chat Interface**: Modern React-based UI with typing indicators
- **Context Awareness**: Maintains conversation history across chat sessions
- **Markdown Support**: Rich text formatting for bot responses
- **Responsive Design**: Built with Tailwind CSS and shadcn/ui components
- **Type Safety**: Full TypeScript implementation for both frontend and backend
- **Modular Architecture**: Clean separation of concerns with proper abstraction

## 🏗️ Architecture

### Backend

- **Express.js** with TypeScript for robust API development
- **OpenAI API Integration** for AI-powered responses
- **Modular Structure**: Routes, Controllers, Services, and Repositories
- **Input Validation** and comprehensive error handling
- **Conversation Management** with unique session IDs

### Frontend

- **React 18** with TypeScript for type-safe development
- **Tailwind CSS** for modern, responsive styling
- **shadcn/ui** components for polished UI elements
- **React Hook Form** for efficient form state management
- **Component-based Architecture** with clear separation of concerns

## 📁 Project Structure

```
├── packages/
│   ├── client/                 # React frontend application
│   │   ├── src/
│   │   │   ├── components/
│   │   │   │   ├── chat/      # Chat-related components
│   │   │   │   └── ui/        # Reusable UI components
│   │   │   ├── lib/           # Utility functions
│   │   │   └── App.tsx        # Main application component
│   │   └── package.json
│   └── server/                 # Express backend application
│       ├── controllers/        # Request handlers
│       ├── services/           # Business logic
│       ├── repositories/       # Data access layer
│       ├── routes.ts          # API route definitions
│       └── index.ts           # Server entry point
├── package.json                # Root package configuration
└── README.md
```

## 🛠️ Tech Stack

- **Frontend**: React, TypeScript, Tailwind CSS, shadcn/ui, React Hook Form
- **Backend**: Node.js, Express, TypeScript, OpenAI API
- **Build Tools**: Vite, Bun
- **Development**: ESLint, TypeScript compiler

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- Bun package manager
- OpenAI API key

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd Chatbot
   ```

2. **Install dependencies**

   ```bash
   bun install
   ```

3. **Set up environment variables**
   Create a `.env` file in the server directory:

   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   PORT=3001
   ```

4. **Start the development servers**

   **Backend (Terminal 1):**

   ```bash
   cd packages/server
   bun run dev
   ```

   **Frontend (Terminal 2):**

   ```bash
   cd packages/client
   bun run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5173` to access the chatbot interface

## 📱 Usage

1. **Start a Conversation**: Type your message in the input field and press Enter
2. **View Responses**: The AI will respond with intelligent, contextual replies
3. **Continue Chatting**: Maintain conversation context across multiple exchanges
4. **Rich Formatting**: Enjoy markdown-formatted responses for better readability

## 🔧 API Endpoints

### POST `/api/chat`

Send a message and receive an AI-generated response.

**Request Body:**

```json
{
   "prompt": "Your message here",
   "conversationId": "optional-conversation-id"
}
```

**Response:**

```json
{
   "response": "AI-generated response",
   "conversationId": "conversation-id"
}
```

## 🏛️ Architecture Principles

This project demonstrates several key software engineering principles:

- **Separation of Concerns**: Clear boundaries between UI, business logic, and data access
- **Abstraction**: Public interfaces hide implementation details
- **Modularity**: Reusable components and services
- **Type Safety**: Full TypeScript implementation for better development experience
- **Error Handling**: Comprehensive error management throughout the stack

## 🎨 Component Architecture

### Frontend Components

- **`ChatBot`**: Main chat container and state management
- **`ChatInput`**: Message input with form validation
- **`ChatMessages`**: Message display with auto-scrolling
- **`TypingIndicator`**: Real-time typing simulation

### Backend Modules

- **Routes**: API endpoint definitions
- **Controllers**: Request/response handling
- **Services**: Business logic and OpenAI integration
- **Repositories**: Data persistence and conversation management

## 🚀 Development

### Available Scripts

**Root:**

```bash
bun install          # Install all dependencies
```

**Client:**

```bash
bun run dev         # Start development server
bun run build       # Build for production
bun run preview     # Preview production build
```

**Server:**

```bash
bun run dev         # Start development server
bun run build       # Build TypeScript
bun start           # Start production server
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenAI for providing the AI API
- The React and Express.js communities
- shadcn/ui for beautiful UI components
- Tailwind CSS for the utility-first CSS framework

---

**Built with ❤️ using modern web technologies**
