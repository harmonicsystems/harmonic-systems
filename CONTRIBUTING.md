# Contributing to Harmonic Systems

Thank you for your interest in contributing! This project exists at the intersection of music, technology, accessibility, and cultural respect. We welcome contributions that align with these values.

## Philosophy First

Before contributing code, please understand our core principles:

### Analog-First Philosophy
- Technology serves human connection, never replaces it
- Digital tools should reduce stimulation, not increase it
- Features that encourage screen time over embodied practice will not be accepted

### Accessibility & Neurodivergence
- Multiple ways to engage with every feature
- No auto-playing media, no sudden animations
- Generous whitespace and clear visual hierarchy
- Processing time and sensory needs respected
- Test with screen readers and keyboard navigation

### Cultural Respect
- All musical traditions must be properly attributed
- Acknowledge when we're guests in another culture's sonic landscape
- Cite sources for traditional materials
- Consult with cultural practitioners when appropriate

### Privacy & Data Ethics
- No tracking or analytics without explicit opt-in
- No selling user data, ever
- Local-first where possible
- Clear data retention policies
- Use privacy-focused alternatives (Plausible over Google Analytics)

## How to Contribute

### Reporting Issues

When reporting bugs or suggesting features:
- Check existing issues first
- Provide clear, minimal reproduction steps
- Include your browser/OS information
- Describe expected vs. actual behavior
- For accessibility issues, specify which assistive technology you're using

### Code Contributions

1. **Fork the repository** and create a feature branch
2. **Follow the existing code style** (we use Prettier + ESLint)
3. **Write clear commit messages** that explain why, not just what
4. **Test on slow connections** (throttle to 3G speeds)
5. **Test with keyboard navigation only**
6. **Update documentation** for any new features

### Pull Request Process

1. Update the README.md if needed
2. Add tests for new functionality
3. Ensure all tests pass
4. Request review from maintainers
5. Be patient and respectful during code review

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/harmonic-systems.git
cd harmonic-systems

# Install dependencies
pnpm install

# Run development server
pnpm dev

# Run tests
pnpm test

# Check accessibility
pnpm a11y
```

## Code Style Guidelines

- **TypeScript**: Prefer type safety over `any`
- **Components**: Functional components with hooks
- **Naming**: Clear, descriptive names over clever ones
- **Comments**: Explain why, not what
- **Complexity**: Simple and readable over clever and compact

## Design Guidelines

### Visual Design
- Muted color palette (#2c3e50, #7f8c8d, earth tones)
- Generous whitespace (24px minimum margins)
- Font sizes: 16px minimum for body text
- Line height: 1.6 minimum for readability
- Contrast ratios: WCAG AAA compliance

### Interaction Design
- Predictable behavior (no surprises)
- Clear feedback for all actions
- Loading states for async operations
- Error messages that explain what to do next
- No time-pressure interactions

### Audio Features
- Volume controls easily accessible
- Visual alternatives for audio cues
- No auto-play
- Clear stop/pause controls
- Respect system audio settings

## Content & Sourcing Guidelines

### All Content Must Include Sources

This is a living repository of curated knowledge. All blog posts, lessons, and informational content **must include a Sources section**. This applies even when:

- Summarizing common knowledge
- Paraphrasing from Wikipedia
- Drawing from personal expertise
- Synthesizing multiple sources

**Why this matters:** We're building a second brain, not claiming original authorship of established knowledge. Readers should always be able to trace ideas back to their origins and dive deeper.

### Citation Format

Use the template in `blog/TEMPLATE.html` as a starting point. Sources sections should:

1. **Be organized by topic** - Group related sources under relevant headings
2. **Mix accessible and academic sources** - Wikipedia, blogs, and videos alongside peer-reviewed papers
3. **Link everything possible** - Make it easy for readers to explore further
4. **Use proper academic format** - For papers: Author. (Year). *Title*. Journal/Publisher.
5. **Include context** - Note if a source is Wikipedia, a documentary, a research paper, etc.

**Example structure:**
```html
<h2>Sources</h2>

<h3>Foundational Concepts</h3>
<ul>
    <li><a href="[URL]">[Topic]</a> (Wikipedia)</li>
    <li>Author. (Year). <em>Title</em>. Publisher.</li>
</ul>

<h3>Specific Research</h3>
<ul>
    <li>Author et al. (Year). Study title. <em>Journal Name</em>, vol(issue), pages.</li>
</ul>
```

### What Needs Sources

- **Blog posts**: Always include Sources section before footer
- **Playlist descriptions**: Cite documentaries, articles, Wikipedia when discussing history/context
- **Lessons**: Reference teaching materials, research, or traditional sources
- **Tools documentation**: Cite relevant standards, APIs, or educational resources

### When Wikipedia Is Enough

Wikipedia is a completely valid source for:
- Defining established concepts (fundamental frequency, harmonic series)
- Historical timelines (music history, instrument development)
- Introductory explanations of scientific phenomena
- Biographical information about musicians/composers

For deeper research or contested topics, supplement Wikipedia with academic papers, books, or primary sources.

## Cultural Contribution Guidelines

When adding content related to musical traditions:

1. **Research thoroughly** - Understand the cultural context
2. **Cite your sources** - Academic, community, or traditional sources
3. **Acknowledge limitations** - Be clear about what you don't know
4. **Invite dialogue** - Create space for corrections and deeper learning
5. **Compensate when appropriate** - If learning from living practitioners, consider payment

### What We Welcome

- Bug fixes and performance improvements
- Accessibility enhancements
- Documentation improvements
- Test coverage additions
- Design system refinements
- Internationalization (i18n) support
- Privacy-enhancing features

### What We Don't Accept

- Features that increase digital stimulation
- Gamification or engagement-maximizing patterns
- Tracking or analytics without explicit opt-in
- Cultural appropriation or misrepresentation
- Paywalled accessibility features
- Performance-pressure features (leaderboards, streaks, etc.)

## Questions?

Not sure if your idea fits? Open an issue to discuss it first! We'd rather talk through an idea early than have you spend time on something that doesn't align with the project's values.

## Code of Conduct

### Our Standards

- Be respectful and inclusive
- Assume good intentions
- Accept constructive criticism gracefully
- Focus on what's best for the community
- Show empathy toward others

### Not Acceptable

- Harassment or discrimination of any kind
- Trolling, insulting, or derogatory comments
- Public or private harassment
- Publishing others' private information
- Other conduct reasonably considered inappropriate

## Recognition

Contributors will be recognized in our README and release notes. We value all contributions - code, documentation, design, testing, and thoughtful discussion.

---

Thank you for helping build technology in service of human resonance.
