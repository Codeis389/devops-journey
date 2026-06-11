# Real Project - Devops Blog

## Day 1: Built Blog

- HTML/CSS professional blog
- git init + pushed to GitHub

## Day 2: Dockerized
- Created Dockerfile
- Built image: docker build -t devops-blog .
- Ran container: docker run -d -p 8081:80 devops-blog

# DAy 3: CI/CD Pipeline

- Created .github/workflows/deploy.yml
- Auto builds Docker image on every push
- Auto tests container
- Auto deploys to GitHub Pages
- Pipeline: push -> build -> test -> deploy
