# Mintlify Documentation Project

## Project Overview

This is a **Mintlify documentation starter kit** - a comprehensive documentation site built with Mintlify that serves as a template for creating beautiful, modern documentation websites. The project includes examples of guides, API reference documentation, and various Mintlify components.

### Key Features

- **Modern Documentation Site**: Built with Mintlify's documentation platform
- **Comprehensive Examples**: Includes guides, API reference, and component examples
- **AI Tools Integration**: Documentation for Cursor, Claude Code, and Windsurf
- **API Documentation**: Complete OpenAPI specification with plant store example
- **Responsive Design**: Light/dark theme support with customizable branding
- **Component Library**: Extensive use of Mintlify components (Cards, Steps, Accordions, etc.)

## Project Structure

```
mintlify-docs/
├── ai-tools/                    # AI development tools documentation
│   ├── claude-code.mdx         # Claude Code setup guide
│   ├── cursor.mdx              # Cursor configuration guide
│   └── windsurf.mdx            # Windsurf setup guide
├── api-reference/              # API documentation
│   ├── endpoint/               # Individual endpoint examples
│   │   ├── create.mdx          # POST endpoint example
│   │   ├── delete.mdx          # DELETE endpoint example
│   │   ├── get.mdx             # GET endpoint example
│   │   └── webhook.mdx         # Webhook endpoint example
│   ├── introduction.mdx        # API overview
│   └── openapi.json            # OpenAPI 3.1.0 specification
├── essentials/                 # Core documentation features
│   ├── code.mdx                # Code examples and syntax highlighting
│   ├── images.mdx              # Image handling and media
│   ├── markdown.mdx            # Markdown/MDX writing guide
│   ├── navigation.mdx          # Navigation structure
│   ├── reusable-snippets.mdx   # Content reuse patterns
│   └── settings.mdx            # Site customization
├── images/                     # Static assets
│   ├── checks-passed.png       # Deployment success image
│   ├── hero-dark.png           # Dark theme hero image
│   └── hero-light.png          # Light theme hero image
├── logo/                       # Branding assets
│   ├── dark.svg                # Dark theme logo
│   └── light.svg               # Light theme logo
├── snippets/                   # Reusable content snippets
│   └── snippet-intro.mdx       # Snippet introduction
├── docs.json                   # Main configuration file
├── favicon.svg                 # Site favicon
├── index.mdx                   # Homepage
├── quickstart.mdx              # Getting started guide
├── development.mdx             # Local development setup
├── LICENSE                     # MIT License
└── README.md                   # Project documentation
```

## Configuration

### Main Configuration (`docs.json`)

The project is configured through `docs.json` which defines:

- **Site Identity**: Name, colors, logos, favicon
- **Navigation Structure**: Tabs, groups, and page organization
- **Theme Settings**: Primary colors (#16A34A green theme)
- **Global Links**: External documentation and blog links
- **Contextual Options**: AI tool integrations (ChatGPT, Claude, Cursor, etc.)
- **Social Links**: Twitter, GitHub, LinkedIn

### Key Configuration Features

- **Two-tab Navigation**: "Guides" and "API reference"
- **AI Tool Integration**: Cursor, Claude Code, Windsurf documentation
- **OpenAPI Integration**: Automatic API documentation generation
- **Responsive Design**: Light/dark theme support
- **Component Library**: Extensive Mintlify component usage

## Setup and Development

### Prerequisites

- Node.js version 19 or higher
- npm package manager
- Git for version control

### Installation

1. **Install Mintlify CLI globally**:
   ```bash
   npm i -g mint
   ```

2. **Navigate to the docs directory**:
   ```bash
   cd mintlify-docs
   ```

3. **Start local development server**:
   ```bash
   mint dev
   ```

4. **View documentation**: Open `http://localhost:3000`

### Custom Port

To run on a different port:
```bash
mint dev --port 3333
```

### Deployment

1. **Install GitHub App**: Connect your repository to Mintlify via the [dashboard](https://dashboard.mintlify.com/settings/organization/github-app)
2. **Push changes**: Changes are automatically deployed when pushed to the default branch
3. **Verify deployment**: Check for "All checks have passed" confirmation

## Content Structure

### Page Types

1. **Guide Pages**: Step-by-step tutorials and explanations
2. **API Reference**: Auto-generated from OpenAPI specifications
3. **Component Examples**: Demonstrations of Mintlify components
4. **AI Tool Guides**: Setup instructions for development tools

### Writing Standards

- **MDX Format**: All content uses MDX (Markdown + JSX)
- **YAML Frontmatter**: Required for page metadata (title, description)
- **Component Usage**: Extensive use of Mintlify components
- **Code Examples**: Syntax-highlighted, language-specific code blocks
- **Responsive Images**: Properly framed and optimized images

## Customization Guide

### Branding

1. **Update `docs.json`**:
   - Change `name` field to your project name
   - Modify `colors` object for brand colors
   - Update `logo` paths for custom logos

2. **Replace Assets**:
   - Update `favicon.svg`
   - Replace logo files in `logo/` directory
   - Add custom images to `images/` directory

### Navigation

Modify the `navigation` section in `docs.json` to:
- Add/remove tabs
- Reorganize page groups
- Update page references
- Add external links

### Content

1. **Create New Pages**: Add `.mdx` files with proper frontmatter
2. **Update Existing Content**: Modify `.mdx` files as needed
3. **Add Components**: Use Mintlify components for enhanced presentation
4. **API Documentation**: Update `openapi.json` for API changes

## Key Components Used

### Structural Components
- **Cards**: Information presentation and navigation
- **Steps**: Sequential instructions
- **Accordions**: Collapsible content sections
- **Tabs**: Platform-specific or alternative content
- **Columns**: Multi-column layouts

### Callout Components
- **Note**: Additional helpful information
- **Tip**: Best practices and pro tips
- **Warning**: Important cautions
- **Info**: Neutral contextual information
- **Check**: Success confirmations

### Code Components
- **CodeGroup**: Multi-language code examples
- **RequestExample/ResponseExample**: API documentation
- **ParamField/ResponseField**: API parameter documentation

### Media Components
- **Frame**: Image containers with optional captions
- **Video**: Self-hosted video content
- **iframe**: Embedded content (YouTube, etc.)

## Development Workflow

### Local Development

1. **Make Changes**: Edit `.mdx` files or `docs.json`
2. **Preview**: Changes appear automatically at `http://localhost:3000`
3. **Test**: Verify all links and components work correctly
4. **Commit**: Use Git to version control changes

### Content Creation

1. **Plan Structure**: Define page hierarchy and navigation
2. **Write Content**: Use MDX with Mintlify components
3. **Add Examples**: Include code samples and visual elements
4. **Review**: Check for clarity, accuracy, and completeness
5. **Deploy**: Push changes for automatic deployment

### Quality Assurance

- **Link Validation**: Use `mint broken-links` to check for broken links
- **Code Testing**: Verify all code examples work correctly
- **Accessibility**: Ensure proper alt text and heading hierarchy
- **Mobile Testing**: Check responsive design on various devices

## Troubleshooting

### Common Issues

1. **Port Already in Use**: Mintlify will automatically use the next available port
2. **Sharp Module Error**: Update to Node.js v19+ and reinstall CLI
3. **Unknown Errors**: Delete `~/.mintlify` folder and restart
4. **404 Pages**: Ensure running in directory with valid `docs.json`

### CLI Updates

Keep CLI updated for latest features:
```bash
npm mint update
```

## Resources

- [Mintlify Documentation](https://mintlify.com/docs)
- [Mintlify Community](https://mintlify.com/community)
- [Mintlify Dashboard](https://dashboard.mintlify.com)
- [MDX VSCode Extension](https://marketplace.visualstudio.com/items?itemName=unifiedjs.vscode-mdx)
- [Prettier Extension](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

## Next Steps

1. **Customize Branding**: Update colors, logos, and site name
2. **Add Your Content**: Replace example content with your documentation
3. **Configure API**: Update OpenAPI specification for your APIs
4. **Set Up Deployment**: Connect GitHub repository for automatic deployment
5. **Enhance Features**: Add custom components and advanced configurations

This project provides a solid foundation for creating professional documentation websites with Mintlify's powerful platform and component library.
