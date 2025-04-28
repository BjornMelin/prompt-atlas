# 🚀 AI-Powered Development Prompts (AIPD)

<!-- Project Status -->

[![MIT License](https://img.shields.io/github/license/BjornMelin/ai-powered-development-prompts?color=green)](LICENSE)
[![Release](https://img.shields.io/github/v/release/BjornMelin/ai-powered-development-prompts?label=release)](https://github.com/BjornMelin/ai-powered-development-prompts/releases)
[![Last Commit](https://img.shields.io/github/last-commit/BjornMelin/ai-powered-development-prompts?color=blue)](https://github.com/BjornMelin/ai-powered-development-prompts/commits)
[![CI](https://img.shields.io/github/actions/workflow/status/BjornMelin/ai-powered-development-prompts/markdown-lint.yml?label=CI&logo=github)](https://github.com/BjornMelin/ai-powered-development-prompts/actions)

<!-- Community -->

[![Open Issues](https://img.shields.io/github/issues/BjornMelin/ai-powered-development-prompts)](https://github.com/BjornMelin/ai-powered-development-prompts/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/BjornMelin/ai-powered-development-prompts)](https://github.com/BjornMelin/ai-powered-development-prompts/pulls)
[![Contributors](https://img.shields.io/github/contributors/BjornMelin/ai-powered-development-prompts)](https://github.com/BjornMelin/ai-powered-development-prompts/graphs/contributors)
[![Star History](https://img.shields.io/github/stars/BjornMelin/ai-powered-development-prompts?style=social)](https://github.com/BjornMelin/ai-powered-development-prompts/stargazers)

<!-- Documentation & Features -->

[![Prompts Library](https://img.shields.io/badge/Prompts-Library-blueviolet?logo=markdown)](./prompts/)
[![Rules Library](https://img.shields.io/badge/Rules-Library-orange?logo=github)](./rules/)
[![Docs](https://img.shields.io/badge/Docs-Available-brightgreen?logo=readthedocs)](./docs/)

Expert-level prompt templates for modern software development using AI pair programming. Optimize your development workflow with carefully crafted prompts for everything from AWS Lambda functions to full-stack applications and AI-powered workflow automation.

## 📋 Table of Contents

- [🚀 AI-Powered Development Prompts (AIPD)](#-ai-powered-development-prompts-aipd)
  - [📋 Table of Contents](#-table-of-contents)
  - [🌟 Features](#-features)
  - [📚 Quick Links](#-quick-links)
  - [🚀 Getting Started](#-getting-started)
  - [📋 Available Templates](#-available-templates)
    - [Cloud Development](#cloud-development)
    - [Frontend Development](#frontend-development)
    - [Backend Development](#backend-development)
    - [Mobile Development](#mobile-development)
    - [Python Development](#python-development)
    - [TypeScript Development](#typescript-development)
    - [CI/CD \& DevOps](#cicd--devops)
  - [🛠️ AI Tools \& Rules](#️-ai-tools--rules)
    - [Cursor AI](#cursor-ai)
    - [GitHub Copilot](#github-copilot)
  - [💡 Example Usage](#-example-usage)
  - [🤝 Contributing](#-contributing)
  - [📈 Best Practices](#-best-practices)
  - [📚 How to Cite](#-how-to-cite)
  - [📜 License](#-license)
  - [🙏 Acknowledgments](#-acknowledgments)
  - [👨‍💻 Author](#-author)
  - [📈 Star History](#-star-history)

## 🌟 Features

- 🎯 **Specialized Templates**: Carefully crafted prompts for different development scenarios
- 🏗️ **Architecture Patterns**: Best practices for modern software design
- ⚡ **Performance Optimization**: Templates focused on scalability and efficiency
- 🔒 **Security First**: Built-in security considerations for each template
- 🚀 **Cloud Native**: Deep integration with modern cloud services
- 📱 **Full Stack**: Coverage from frontend to backend to mobile
- 🤖 **AI Development**: Optimized workflows for AI-assisted development
- 🔄 **CI/CD**: Continuous integration and deployment templates
- 💻 **IDE Integration**: Custom rules for AI coding assistants like Cursor

## 📚 Quick Links

- [🌟 Features](#-features)
- [Getting Started](#-getting-started)
- [Available Templates](#-available-templates)
- [Prompts Library](./prompts/)
- [Rules Library](./rules/)
- [AI Tools & Rules](#️-ai-tools--rules)
- [Docs](./docs/)
- [Best Practices](./docs/best-practices.md)
- [Contributing](#-contributing)
- [License](#-license)

## 🚀 Getting Started

1. **Choose Your Template**

   ```bash
   # Navigate to the relevant category
   prompts/             # Development prompts by category
   ├── cloud/           # Cloud-specific prompts (AWS, Azure, GCP)
   ├── frontend/        # Frontend development templates
   ├── backend/         # Backend and API templates
   ├── mobile/          # Mobile development prompts
   ├── python/          # Reusable expert Python prompts
   └── typescript/      # Reusable expert TypeScript Prompts

   rules/               # AI tool rules and automation
   ├── cursor-ai-agent/ # Autonomous AI agent for Cursor
   ├── cursorrules/     # Rules for Cursor AI coding assistant
   └── copilot/         # GitHub Copilot optimization
   ```

2. **Customize Your Prompt**

   - Replace placeholder values with your specific requirements
   - Follow the examples provided in each template
   - Add or remove sections based on your needs

3. **Execute Your Development Plan**
   - Use the prompts with your preferred AI assistant
   - Follow the structured approach for consistent results
   - Iterate based on feedback and results

## 📋 Available Templates

### Cloud Development

- [AWS Lambda Functions](./prompts/cloud/aws-lambda.md)
- [Serverless Applications](./prompts/cloud/serverless.md)
- [Cloud Architecture](./prompts/cloud/architecture.md)

### Frontend Development

- [React Applications](./prompts/frontend/react.md)
- [Performance Optimization](./prompts/frontend/performance.md)
- [Component Architecture](./prompts/frontend/components.md)

### Backend Development

- [API Design](./prompts/backend/api.md)
- [Database Optimization](./prompts/backend/database.md)
- [Microservices](./prompts/backend/microservices.md)

### Mobile Development

- [React Native](./prompts/mobile/react-native.md)
- [Flutter](./prompts/mobile/flutter.md)
- [Native Apps](./prompts/mobile/native.md)

### Python Development

- [Expert-level Python Prompts](./prompts/python/)

### TypeScript Development

- [Expert TypeScript Prompts (Next.js, React)](./prompts/typescript/)

### CI/CD & DevOps

- [CI/CD Pipeline Templates](./prompts/cicd/)

## 🛠️ AI Tools & Rules

### Cursor AI

- [Ultimate Cursor AI Agent Template](./rules/cursor-ai-agent/) - Autonomous AI development framework
- [Git Feature Workflow](./rules/cursorrules/git_feature_workflow.mdc) - Conventional commits and branch workflow

### GitHub Copilot

- [Prompt Engineering Techniques](./rules/copilot/) - Optimize Copilot interactions

## 💡 Example Usage

```markdown
I need to develop an AWS Lambda function for image processing with:

1. Function Specifications:
   - Runtime: Python 3.11
   - Memory allocation: 1024 MB
     ...

[See full example in docs/examples/lambda-image-processor.md]
```

## 🤝 Contributing

Your contributions are always welcome! See our [Contribution Guidelines](CONTRIBUTING.md) for ways to get started.

We accept:

- 📝 New prompt templates
- 🎨 Template improvements
- 📚 Documentation updates
- 💻 Example implementations
- 🐛 Bug fixes
- 🤖 AI tool configurations

## 📈 Best Practices

- Keep prompts specific and actionable
- Include clear requirements and constraints
- Follow the provided structure
- Add examples where possible
- Consider scalability and maintenance

## 📚 How to Cite

If you use these templates in your research or publications, please cite this repository:

```bibtex
@misc{melin2025aiprompts,
  author = {Melin, Bjorn},
  title = {AI-Powered Development Prompts},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub Repository},
  howpublished = {\url{https://github.com/BjornMelin/ai-powered-development-prompts}}
}
```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- All contributors who have helped improve these templates
- The AI/ML community for valuable feedback
- Open source projects that inspired this collection
- [Bhartendu-Kumar/rules_template](https://github.com/Bhartendu-Kumar/rules_template) and [kleosr/cursorkleosr](https://github.com/kleosr/cursorkleosr) for inspiration on the Cursor AI Agent system

---

## 👨‍💻 Author

**Bjorn Melin**  
Senior Data Scientist · AI/ML Leader · GenAI & LLM Expert · UC Berkeley MIDS · 6x AWS Certified · Cloud Architect & Full-Stack Developer at heart!

- 🌐 [bjornmelin.io](https://bjornmelin.io)
- 🐙 [GitHub](https://github.com/BjornMelin)
- 💼 [LinkedIn](https://www.linkedin.com/in/bjorn-melin/)

## 📈 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=BjornMelin/ai-powered-development-prompts&type=Date)](https://star-history.com/#BjornMelin/ai-powered-development-prompts&Date)

<p align="center">Made with 🤖 by developers, for developers.</p>
