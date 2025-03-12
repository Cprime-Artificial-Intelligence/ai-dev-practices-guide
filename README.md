# AI Development Practices Guide

This repository contains a comprehensive guide to best practices and anti-patterns in AI development.

## Documentation

The documentation is built using [MkDocs](https://www.mkdocs.org/) with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

### View the Documentation

The documentation is automatically deployed to GitHub Pages and can be viewed at:
https://cprime-artificial-intelligence.github.io/ai-dev-practices-guide/

### Local Development

To run the documentation locally:

#### Option 1: Using the setup script (recommended)

1. Clone this repository:
   ```bash
   git clone https://github.com/Cprime-Artificial-Intelligence/ai-dev-practices-guide.git
   cd ai-dev-practices-guide
   ```

2. Run the setup script:
   - On Linux/macOS:
     ```bash
     ./setup_and_test.sh
     ```
   - On Windows:
     ```bash
     setup_and_test.bat
     ```

3. Start the local development server:
   - On Linux/macOS:
     ```bash
     source venv/bin/activate
     mkdocs serve
     ```
   - On Windows:
     ```bash
     venv\Scripts\activate
     mkdocs serve
     ```

4. Open your browser and navigate to `http://localhost:8000`

5. When you're done, deactivate the virtual environment:
   - On Linux/macOS:
     ```bash
     deactivate
     ```
   - On Windows:
     ```bash
     deactivate
     ```

#### Option 2: Manual setup

1. Clone this repository:
   ```bash
   git clone https://github.com/Cprime-Artificial-Intelligence/ai-dev-practices-guide.git
   cd ai-dev-practices-guide
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Start the local development server:
   ```bash
   mkdocs serve
   ```

5. Open your browser and navigate to `http://localhost:8000`

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Deployment

The deployment process works in two stages:

1. **GitHub Actions Workflow**: When changes are pushed to the main branch, a GitHub Actions workflow builds the MkDocs site and pushes the generated content to the `gh-pages` branch.

2. **GitHub Pages**: GitHub's built-in Pages service then detects changes to the `gh-pages` branch and deploys the content to the public site at https://cprime-artificial-intelligence.github.io/ai-dev-practices-guide/.

This two-stage process ensures that your documentation is always up-to-date with the content in your main branch.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
