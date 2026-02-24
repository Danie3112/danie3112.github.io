# COSESCO Web Project - AI Coding Guidelines

## Project Overview
This is a static website for COSESCO, a financial cooperative. The site consists of a single HTML page with sections for services, requirements, and contact information.

## Architecture
- **Single-page design**: All content in `index.html` with anchor-linked sections (#inicio, #nosotros, #servicios, etc.)
- **Styling**: Centralized in `css/estilos.css` with responsive breakpoints
- **Minimal JavaScript**: Inline script in `<head>` for mobile menu toggle

## Key Conventions
- **Language**: All content and comments must be in Spanish
- **Color scheme**: Primary blue `#0a4c8b`, light backgrounds `#f4f6f8`, text `#333`
- **Layout**: Flexbox-based responsive design with mobile-first approach
- **Navigation**: Anchor links for internal sections, no routing framework

## Development Patterns
- **HTML structure**: Header → sections → footer, each section with `id` for navigation
- **CSS organization**: Reset → body → header → nav → sections → responsive
- **Responsive**: Hide/show menu with `.menu-toggle` and `.show` class toggle
- **Forms**: Simple HTML forms without validation (e.g., contact form in `#contacto`)

## File Structure
- `index.html`: Main page with all content and inline JS
- `css/estilos.css`: All styles including responsive rules
- Images: Referenced as `img/logo-cosesco.png` (create `img/` directory if needed)

## Common Tasks
- **Add new section**: Insert `<section id="new-section">` before footer, add nav link
- **Update colors**: Modify hex values in `:root` or directly in selectors
- **Mobile optimization**: Test `@media (max-width: 768px)` rules
- **Content updates**: Maintain Spanish language and cooperative-focused messaging

## Examples
- **Section addition**: `<section id="nueva-seccion"><h2>Nuevo Título</h2><p>Contenido...</p></section>`
- **Service cards**: Use `.servicio` class with flex container for consistent styling
- **Button styling**: Apply `background-color: #0a4c8b; color: #fff;` for CTAs</content>
<parameter name="filePath">c:\Users\yanis\OneDrive\Documentos\cosesco-web\.github\copilot-instructions.md