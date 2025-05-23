# Docker-and-github-cicd-project3

# Containerized Static Site with CSS and CI/CD Testing

A styled static site (HTML/CSS) containerized with Docker, automated via GitHub Actions CI/CD with testing, built on a mobile device.

## Features
- Styled site served by Nginx.
- CI/CD pipeline with file existence tests.
- Pushes to `sandwich5230/my-static-site-two:latest`.

## How to Run
1. Clone: `git clone https://github.com/rudesandwich/Test-docker-cicd-repo-two.git`
2. Build: `docker build -t sandwich5230/my-static-site-two:latest .`
3. Run: `docker run -p 8080:80 sandwich5230/my-static-site-two:latest`
4. Open `localhost:8080`.

## CI/CD Workflow
- Triggers on `main` branch pushes.
- Tests: Verifies `index.html` and `style.css` exist.
- Builds and pushes Docker image.

## Next Steps
- Deploy live on Oracle Cloud.
- Add JavaScript for interactivity.