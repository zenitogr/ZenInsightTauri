# ZenInsightTauri Development Documentation

## Project Overview

ZenInsightTauri is an offline-first Android application designed to educate users about their phone's technology, privacy, and data collection practices.

## Core Objectives

- Create a 100% offline educational tool
- Provide clear explanations about phone permissions
- Analyze and explain data collection practices of popular apps
- Educate users about advertisement tracking
- Explain mobile technologies (RCS, phone app behaviors, etc.)

## Technical Stack

### Frontend
- Vue.js with TypeScript
- TailwindCSS
- Shadcn/UI components
- Vue Router for navigation
- Vuex for state management
- Vue-i18n for internationalization
- Vite for build tooling

### Backend
- Rust (Tauri)
- Local storage only
- No external API dependencies

## Development Phases

### Phase 1: Foundation (v0.0.1)

1. **Project Setup**
   ```bash
   cargo install create-tauri-app
   cargo create-tauri-app
   ```

2. **Basic Structure**
   ```
   src/
   ├── components/
   │   ├── PermissionExplainer/
   │   ├── DataCollectionAnalyzer/
   │   └── TechnologyGuide/
   ├── views/
   ├── store/
   └── i18n/
   ```

### Phase 2: Core Features

#### Permission Education Module
- Comprehensive permission database
- User-friendly permission explanations
- Real-world usage examples
- Privacy implications

#### App Analysis Features
- Facebook data collection practices
- Twitter data tracking
- Messenger permissions
- Viber privacy analysis
- Advertisement tracking explanations

#### Technology Education
- RCS messaging explanation
- Phone app behavior analysis
- Mobile technology glossary
- Privacy guides

## Implementation Guidelines

### Offline-First Architecture

#### Local Storage Strategy
- All educational content stored locally
- No external API calls
- Efficient data organization

#### Content Management
- Static content bundling
- Markdown-based documentation
- Embedded resources

### Privacy-Focused Development

#### Zero Data Collection
- No analytics
- No external services
- No user tracking

#### Transparency
- Open source codebase
- Clear documentation
- Explained functionality

## Getting Started

### Prerequisites

1. **Rust toolchain**
   ```bash
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```

2. **Node.js and npm**
   - Install as per your OS

3. **Project setup**
   ```bash
   npm install
   ```

### Development Workflow

1. **Run development server**
   ```bash
   npm run tauri dev
   ```

2. **Build for Android**
   ```bash
   npm run tauri android build
   ```

## Contributing

### Code Style
- Follow Vue.js style guide
- Use Rust formatting guidelines
- Document all components

### Pull Requests
- Create feature branches
- Include tests
- Update documentation

## Resources

- [Project Repository](https://github.com/zenitogr/ZenInsightTauri)
- [Tauri Documentation](https://tauri.app/)
- [Vue.js Guide](https://vuejs.org/)