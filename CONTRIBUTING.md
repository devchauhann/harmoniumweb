# Contributing to Web Harmonium 🎵

Thank you for your interest in contributing to Web Harmonium! We welcome contributions from everyone. This document provides guidelines and information on how to contribute.

## Code of Conduct

Be respectful, inclusive, and constructive. We're all here to learn and build something amazing together!

## Ways to Contribute

### 1. 🐛 Report Bugs

Found a bug? Help us fix it!

- **Check existing issues** first - your bug might already be reported
- **Create a clear issue** with:
  - What happened (description)
  - Steps to reproduce
  - Expected behavior
  - Actual behavior
  - Browser & OS information
  - Screenshots/recordings if applicable

**Bug Report Template:**
```
### Description
Brief description of the bug

### Steps to Reproduce
1. ...
2. ...
3. ...

### Expected Behavior
What should happen

### Actual Behavior
What actually happens

### Environment
- Browser: Chrome 120
- OS: macOS 14
- Screen size: 1920x1080
```

### 2. 💡 Suggest Features

Have an idea to improve Web Harmonium?

- **Describe the feature** clearly
- **Explain the benefit** - how does it help users?
- **Provide examples** - show how it would work
- **Consider alternatives** - are there other ways to implement it?

**Feature Request Template:**
```
### Feature Description
What would you like to add?

### Motivation
Why is this feature valuable?

### Examples
How would users interact with this?

### Alternative Solutions
Any other ways to solve this?
```

### 3. 📝 Improve Documentation

- Enhance README with more examples
- Fix typos or unclear explanations
- Add tutorials for getting started
- Translate documentation to other languages

### 4. 🎨 Design & UI Improvements

- Visual enhancements
- Better mobile responsiveness
- Accessibility improvements (a11y)
- Color scheme variations

### 5. 🔧 Code Improvements

- Performance optimizations
- Code refactoring
- Adding tests
- Fixing technical debt

### 6. 🌍 Translations

Help make Web Harmonium accessible globally! Consider translating:
- README
- UI text
- Documentation
- Comments

## Development Setup

### Prerequisites
- A modern web browser (Chrome 90+, Firefox 88+, Safari 14+)
- A text editor (VS Code recommended)
- Git

### Local Development

```bash
# 1. Fork the repository on GitHub
# 2. Clone your fork locally
git clone https://github.com/YOUR_USERNAME/harmoniumweb.git
cd harmoniumweb

# 3. Create a feature branch
git checkout -b feature/your-feature-name

# 4. Start a local server
python3 -m http.server 8000
# or
npx http-server

# 5. Open http://localhost:8000 in your browser
```

### Testing Your Changes

- Test in multiple browsers (Chrome, Firefox, Safari)
- Test on mobile devices (landscape mode)
- Test with MIDI devices if modifying MIDI code
- Check keyboard responsiveness

## Submitting Changes

### Before You Submit

1. **Test thoroughly** in multiple browsers
2. **Check for console errors** (open DevTools)
3. **Verify mobile responsiveness** (responsive mode)
4. **Review your code** for clarity and comments
5. **Keep commits atomic** (one logical change per commit)

### Pull Request Process

1. **Update README** if you've added new features
2. **Add comments** to complex code sections
3. **Write clear commit messages**:
   ```
   git commit -m "Add feature: descriptive message"
   ```
4. **Push to your fork**:
   ```
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request** on GitHub with:
   - Clear title describing the change
   - Description of what was changed and why
   - Reference to related issues if applicable
   - Screenshots if UI changes were made

### PR Template

```
## Description
What does this PR do?

## Related Issues
Closes #(issue number)

## Changes Made
- Change 1
- Change 2
- Change 3

## Screenshots/Demo
(if applicable)

## Testing
How was this tested? What browsers/devices?

## Checklist
- [ ] Code tested in multiple browsers
- [ ] Mobile responsiveness checked
- [ ] No console errors
- [ ] Comments added to complex code
- [ ] README updated if needed
```

## Code Style Guidelines

### General Principles
- **Readability first** - Write clear, understandable code
- **Keep it simple** - Avoid unnecessary complexity
- **DRY (Don't Repeat Yourself)** - Extract repeated code
- **Comments matter** - Explain the "why" not the "what"

### JavaScript Style
```javascript
// Use meaningful variable names
const harmoniumVolume = 80; // Good
const vol = 80; // Avoid

// Add comments for non-obvious logic
// Exponential volume scaling for more natural feel
const scaledVolume = Math.pow(volume / 100, 2);

// Use template literals
const message = `Playing note ${note} at octave ${octave}`; // Good
const message = 'Playing note ' + note + ' at octave ' + octave; // Avoid

// Consistent formatting
function playNote(frequency, duration) {
  // ...
}

// Bad
function playNote(frequency,duration){
  // ...
}
```

### CSS Style
```css
/* Use CSS variables for consistency */
color: var(--text);
background: var(--bg);

/* Meaningful class names */
.control-panel { /* Good */
  /* styles */
}

.cp { /* Avoid */
  /* styles */
}

/* Group related properties */
.button {
  /* Layout */
  display: flex;
  align-items: center;
  
  /* Sizing */
  width: 100%;
  height: 40px;
  
  /* Styling */
  background: var(--accent);
  color: var(--text);
}
```

## File Organization

### Single File Structure
Web Harmonium uses a single `index.html` for simplicity:
- CSS goes in `<style>` tags (top of `<head>`)
- HTML structure in `<body>`
- JavaScript in `<script>` tags (end of `<body>`)

### Sections in index.html
```html
<!-- 1. Meta tags & SEO -->
<!-- 2. CSS variables & styles -->
<!-- 3. HTML structure -->
<!-- 4. JavaScript -->
```

## Performance Considerations

- Minimize re-renders
- Avoid blocking operations
- Use efficient selectors
- Cache DOM queries
- Test with DevTools Performance tab

## Accessibility (a11y)

- Ensure keyboard navigation works
- Use semantic HTML
- Add ARIA labels where needed
- Test with screen readers
- Maintain good color contrast

## Questions?

- Check existing issues and discussions
- Open a new discussion if unsure
- Reach out on GitHub
- Comment on related issues for guidance

## Recognition

Contributors will be recognized in:
- GitHub contributors page
- README acknowledgments
- Release notes

## Resources

- [Web Audio API Docs](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [Web MIDI API](https://developer.mozilla.org/en-US/docs/Web/API/Web_MIDI_API)
- [HTML5 Specification](https://html.spec.whatwg.org/)
- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)

---

**Thank you for contributing! 🙏**

Together we're building something amazing. Let's make Web Harmonium the best online harmonium player! 🎵
