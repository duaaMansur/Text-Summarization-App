# Text-Summarization-App: CI/CD for ML Model Deployment on Hugging Face Spaces

This repository contains a **Text Summarization Application** with continuous integration and deployment (CI/CD) setup using **GitHub Actions**. The project focuses on deploying a machine learning model for text summarization on **Hugging Face Spaces**.

## Features

- **CI/CD Pipeline**: Automates the deployment process of the machine learning model
- **Hugging Face Spaces Deployment**: Easily deploy the model on Hugging Face for fast inference
- **Local Development**: Use your local environment to build, test, and prepare the model before pushing to the repository

## How it Works

1. **Model Development**: Develop and train a text summarization model locally
2. **Push Code to GitHub**: Once the model is ready, push your code to the GitHub repository
3. **CI/CD with GitHub Actions**: Upon each push, GitHub Actions automatically triggers the pipeline to test, build, and deploy the model to Hugging Face Spaces
4. **Deployment to Hugging Face**: The model will be deployed on Hugging Face Spaces for easy access and usage

## Prerequisites

- Python 3.x
- GitHub account
- Hugging Face account

## Setup

1. Clone the repository
2. Set up your Hugging Face credentials
3. Add your model to the appropriate directory
4. Configure the GitHub Actions workflow for deployment

## Installation

```bash
# Clone the repository
git clone https://github.com/duaaMansur/Text-Summarization-App
cd Text-Summarization-App

# Install dependencies
pip install -r requirements.txt
```

## Configuration

### Hugging Face Credentials

1. Create a Hugging Face account at [huggingface.co](https://huggingface.co)
2. Generate an access token from your Hugging Face account settings
3. Add the token to your GitHub repository secrets:
   - Go to your GitHub repository
   - Navigate to Settings → Secrets and variables → Actions
   - Add a new secret named `HF_TOKEN` with your Hugging Face token

### GitHub Actions Workflow

The CI/CD pipeline is configured in `.github/workflows/deploy.yml`. This workflow:
- Triggers on push to the main branch
- Sets up Python environment
- Installs dependencies
- Runs tests
- Deploys to Hugging Face Spaces


## Usage

### Local Development

```bash
# Run the application locally
python app/main.py

# Run tests
python -m pytest tests/
```

### Deployment

1. Push your changes to the main branch
2. GitHub Actions will automatically trigger the deployment
3. Your model will be available on Hugging Face Spaces


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References

[Watch YouTube Walkthrough](https://youtu.be/VYSGjUa5sc4)
