ZenInsightTauri - Development Guide - v0.0.2 (2024-03-19)

# Quick Start Guide

## Setup Requirements

### 1. Basic Tools
- Windows 10/11 with WSL2
- Android Studio
- VS Code
- Node.js LTS
- JDK 17+

### 2. Development Tools
```bash
# Install Rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Add Android targets
rustup target add aarch64-linux-android armv7-linux-androideabi

# Install dependencies
npm install
```

## Project Structure

```
src/              # Vue frontend
  ├─ views/       # Main screens
  ├─ components/  # Reusable parts
  └─ i18n/        # Translations

src-tauri/        # Rust backend
  ├─ src/         # Core logic
  └─ android/     # Android specific
```

## Common Tasks

### Development
```bash
# Start development
cargo tauri android dev

# Build release
cargo tauri android build
```

### Testing
```bash
# Run unit tests
npm run test

# Run e2e tests
npm run test:e2e
```

## Feature Implementation Guide

### Adding New Content
1. Create markdown file in `content/`
2. Add translations in `i18n/`
3. Create view component
4. Add to navigation

### Creating UI Components
1. Use Shadcn/UI base
2. Follow Vue composition API
3. Add TypeScript types
4. Include unit tests

## Troubleshooting

### Common Issues
- **Build fails**: Check Android SDK path
- **Emulator crashes**: Update Android Studio
- **Hot reload not working**: Restart dev server

### Getting Help
- Check GitHub issues
- Join Discord community
- Read Tauri docs

## Best Practices

### Code Style
- Use TypeScript strictly
- Follow Vue composition API
- Document all functions
- Write unit tests

### Git Workflow
- Feature branches
- Descriptive commits
- PR templates
- Code review checklist