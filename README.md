# Agent Rules Recipes

A repository of pre-built project recipes for the Agent Rules Generator. Each recipe defines a project type with metadata, technology stacks, and configuration rules to streamline AI-assisted development workflows.

## 📁 Project Structure

```
agent-rules-recipes/
├── recipes/               # Project recipe files (.yaml)
│   ├── apollo-graphql-api.yaml
│   ├── express-rest-api.yaml
│   ├── rbac-trpc-react.yaml
│   ├── react_recipe.yaml
│   └── react-node-mongodb.yaml
└── templates/             # Template files referenced by recipes
    ├── agent-template.md
    ├── general-template.md
    ├── node-backend-template.md
    └── react-app-template.md
```

## 📚 Recipe Format

Recipes are YAML files containing:
- `name`: Project type identifier
- `description`: Brief project purpose
- `category`: Frontend/Backend/Full Stack
- `tags`: Technology-specific tags
- `techStack`: Object defining language, frameworks, and tools
- `templates`: Mapping of template files to output paths

Example:
```yaml
name: "React + Node.js + MongoDB"
description: "Full-stack application with React frontend and Node.js backend using MongoDB"
category: "Full Stack"
tags:
  - react
  - node
  - mongodb
techStack:
  language: "JavaScript/TypeScript"
  frontend: "React"
  backend: "Node.js"
  database: "MongoDB"
templates:
  - source: "templates/react-app-template.md"
    target: "{{project_name}}/frontend"
  - source: "templates/node-backend-template.md"
    target: "{{project_name}}/backend"
```

## 🧩 Using Recipes

1. **With Agent Rules Generator**:
   - The generator automatically uses this repo by default
   - Configure a custom repo using: `bun run start` → "Configure remote repository"

2. **Recipe Structure**:
   - YAML files define project configurations
   - Templates provide base structure for generated files

3. **Template Format**:
   - Markdown files with placeholders (e.g., `{{project_name}}`)
   - Used to generate `.agent.md` and `.windsurfrules` files

## 🤝 Contributing Recipes

1. Fork this repository
2. Add new YAML files to the `recipes/` directory
3. Ensure:
   - Clear descriptions
   - Proper categorization
   - Consistent formatting
   - Relevant metadata
4. Submit a pull request with a clear description

## 📄 License

This project is licensed under the GNU General Public License (GPL) - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by the need for standardized AI development workflows
- Built with contributions from the Cursor AI and Windsurf communities
- Special thanks to the developers of the Agent Rules Generator
