---
name: frontend-design
description: Create distinctive, production-grade frontend interfaces with high design quality and intentional aesthetics. Use when building web components, pages, applications, posters, landing pages, dashboards, or any UI interface that requires thoughtful design. Generates creative, polished code that avoids generic AI-generated aesthetics.
license: Apache 2.0
---

## Purpose

This skill transforms frontend design tasks into visually striking, production-ready interfaces that avoid generic "AI-generated" aesthetics. It provides frameworks and guidelines for creating memorable, context-specific designs through intentional aesthetic choices.

## When to Use This Skill

Use this skill when:
- Building new web components, pages, or applications
- Creating landing pages, dashboards, or admin interfaces
- Designing posters, cards, banners, or visual artifacts
- Styling or beautifying existing web UI
- Working with HTML/CSS layouts, React components, or Vue interfaces
- Any task requiring visual design decisions

## Design Thinking Process

Before writing code, establish a clear creative direction:

### 1. Understand Context
- **Purpose**: What problem does this interface solve? Who is the audience?
- **Technical Constraints**: Framework requirements (HTML/React/Vue), performance needs, accessibility requirements
- **Differentiation**: What will make this design unforgettable? What is the single element users will remember?

### 2. Choose an Aesthetic Direction
Commit to one bold aesthetic extreme. Consider:
- **Minimalist**: Brutally clean, generous whitespace, refined details
- **Maximalist**: Vibrant colors, elaborate patterns, rich decorations
- **Retro-futuristic**: Neon, glitch effects, cyberpunk aesthetics
- **Organic**: Natural textures, soft curves, earth tones
- **Luxury/Refined**: Elegant typography, sophisticated palette, subtle gradients
- **Playful/Toy-like**: Rounded shapes, bright colors, playful animations
- **Editorial/Magazine**: Large typography, dramatic layouts, bold imagery
- **Brutalist**: Raw aesthetics, visible grids, high contrast
- **Art Deco**: Geometric patterns, metallic colors, elegance
- **Soft/Pastel**: Gentle hues, blurred elements, dreamy atmosphere
- **Industrial/Utilitarian**: Functional aesthetics, monospace fonts, stark contrasts

**CRITICAL**: Choose ONE direction and execute with precision. Intentionality matters more than intensity.

### 3. Implementation Matching

Match code complexity to the aesthetic vision:
- **Maximalist designs**: Extensive animations, elaborate effects, rich decorations
- **Minimalist designs**: Restraint, precision, careful spacing, subtle details
- **Elegance** comes from executing the chosen vision well

## Frontend Aesthetics Guidelines

### Typography
- Choose distinctive, beautiful fonts that elevate the design
- Avoid generic fonts: Arial, Inter, Roboto, system fonts
- Pair a unique display font with a refined body font
- Consider font families that match the chosen aesthetic
- Examples: Playfair Display for elegance, Space Grotesk for modern, Courier Prime for industrial

### Color & Theme
- Commit to a cohesive aesthetic using CSS variables for consistency
- Use dominant colors with sharp accents rather than evenly-distributed palettes
- Define color system in `:root` for maintainability
- Consider light vs dark theme based on aesthetic direction
- Avoid cliched color schemes (purple gradients on white backgrounds)

### Motion & Animation
- Use animations strategically for high-impact moments
- Prioritize CSS-only solutions for HTML
- Use Motion library (Framer Motion, framer-motion) for React when available
- Focus on orchestrated page loads with staggered reveals (animation-delay)
- Add scroll-triggered animations for dynamic storytelling
- Create surprising hover states that delight users
- Avoid scattered micro-interactions that feel random

### Spatial Composition
- Break predictable grid patterns intentionally
- Use asymmetry for visual interest
- Create overlapping elements for depth
- Consider diagonal flow instead of horizontal layouts
- Break grid elements for emphasis
- Either use generous negative space OR controlled density
- Avoid centering everything without purpose

### Backgrounds & Visual Details
- Create atmosphere and depth, never default to solid colors
- Match effects to overall aesthetic direction
- Techniques to consider:
  - Gradient meshes for organic feel
  - Noise textures for industrial look
  - Geometric patterns for art deco
  - Layered transparencies for modern depth
  - Dramatic shadows for luxury
  - Decorative borders for editorial style
  - Custom cursors for playful interfaces
  - Grain overlays for retro feel

## Anti-Patterns to Avoid

NEVER use generic AI-generated aesthetics:
- Overused font families (Inter, Roboto, Arial, system fonts)
- Cliched color schemes (purple gradients, blue-to-pink fades)
- Predictable layouts and component patterns
- Cookie-cutter designs lacking context-specific character
- Converging on common choices across generations

## Design Principles

1. **Context is King**: Every design decision should serve the specific use case
2. **Vary Output**: Never repeat the same aesthetic twice
3. **Bold Choices**: Commit to decisions rather than hedging with safe options
4. **Detail Obsession**: Refine every pixel, transition, and interaction
5. **Surprise**: Include moments that users don't expect but love
6. **No Templates**: Each design should feel bespoke

## Implementation Workflow

1. **Establish Direction**: Write down the aesthetic choice before coding
2. **Set Variables**: Define CSS variables for colors, fonts, spacing
3. **Build Structure**: Create HTML/JSX with semantic, accessible markup
4. **Apply Styling**: Implement the chosen aesthetic systematically
5. **Refine Details**: Polish animations, hover states, responsive behavior
6. **Test Interactions**: Ensure animations feel smooth and intentional
7. **Review**: Does this match the original aesthetic direction?

## Remember

Claude is capable of extraordinary creative work. Don't hold back—demonstrate what's possible when thinking outside the box and committing fully to a distinctive vision. Great design comes from bold choices and meticulous execution, not safe compromises.
