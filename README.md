# GemmaPoweredResumeBuilder

An intelligent, secure, and privacy-first resume optimization tool powered by Google Gemma. Build modern Angular applications running on top of local generative artificial intelligence.

This application allows software engineers, developers, and professionals to input their existing resume bullet points or job experience descriptions and receive beautifully polished, high-impact, and action-oriented rewrites tailored specifically to tech industry standards.

![Resume Wording Improver Screenshot](public/screenshot.png)

---

## Key Features

- **Local GenAI Processing**: Completely private, secure, and offline. Your resume data never leaves your computer, as all generations are performed locally.
- **Factual Integrity**: Built with strict constraints that forbid the AI from exaggerating, inventing, or fabricating experience or metrics. It preserves your exact facts while putting your best foot forward.
- **Modern Angular Architecture**: Fully designed using modern Angular best practices, including:
  - Responsive layout built with CSS transitions and fade-in animations.
  - Signal-based state management (`signal()`, `computed()`) for maximum efficiency.
  - Angular's built-in template control flow (`@if` / `@else`) for elegant rendering.
- **Structured Routing (PersonalAISpecs)**: Contains persistent instructions, workflows, and specifications structured in the `PersonalAISpecs/` directory.

---

## How It Works

GemmaPoweredResumeBuilder communicates directly with [Ollama](https://ollama.com/), a local LLM runner, to execute the `gemma4` model. The frontend app sends carefully crafted prompt instructions to Ollama's local generation endpoint to ensure that your experience is polished for tech hiring managers without compromising the truth.

---

## Getting Started

Follow these steps to run the application locally.

### Prerequisites

1. Install [Node.js](https://nodejs.org/) (v18 or newer recommended).
2. Install [Ollama](https://ollama.com/).
3. Pull the `gemma4` model locally on your machine:
   ```bash
   ollama pull gemma4
   ```
4. **CRITICAL REQUIREMENT**: You **MUST** ensure Ollama is actively running the `gemma4` model locally before starting the app or sending suggestions. Every time before you start the development server, run the model in your terminal:
   ```bash
   ollama run gemma4
   ```

### Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/DeveloperMattC/GemmaPoweredResumeBuilder.git
   cd GemmaPoweredResumeBuilder
   ```

2. Install the package dependencies:
   ```bash
   npm install
   ```

### Development Server

Start a local development server:

```bash
npm run start
# or
ng serve
```

Once the server is running, open your web browser and navigate to `http://localhost:4200/`.

### Run Unit Tests

To execute unit tests using the modern [Vitest](https://vitest.dev/) test runner, run:

```bash
npm run test
# or
ng test
```

### Production Build

To compile the application for production deployment, run:

```bash
npm run build
# or
ng build
```

The compiled build artifacts will be stored in the `dist/` directory.

