# Trivia Search Website

![GitHub repo size](https://img.shields.io/github/repo-size/yodigi7/trivia-frontend)
![GitHub contributors](https://img.shields.io/github/contributors/yodigi7/trivia-frontend)

## Overview

This repository contains the frontend code for a basic trivia website that allows users to search for trivia questions using natural language queries. The website uses a free Hugging Face Sentence Transformer model to encode both the question/answer pairs and the user's query to find the best match.

## Features

- Search trivia questions using natural language queries.
- Utilizes a Hugging Face Sentence Transformer model to improve search accuracy.
- User-friendly Svelte-based frontend.

## Getting Started

These instructions will help you set up a local development environment for the frontend of the trivia website.

1. **Prerequisites**

   - Node.js and npm installed on your machine.

2. **Clone the Repository**

   ```bash
   git clone https://github.com/yodigi7/trivia-frontend.git
   ```

3. **Install Dependencies**

   ```bash
   cd trivia-frontend
   npm install
   ```

4. **Start the Development Server**

   ```bash
   npm run dev
   ```

5. **Open the Website**
   Your website should be running at [http://localhost:5173](http://localhost:5173).

## How to Use

1. Enter your trivia question or query in the search bar.
2. The website will use the Hugging Face Sentence Transformer model to find the best-matching trivia questions.
3. Browse the results and enjoy!

## Contributing

If you would like to contribute to this project, feel free to create a pull request. We welcome contributions to improve the website's functionality and user experience.

## Acknowledgments

- [Hugging Face Sentence Transformer](https://huggingface.co/models): We used a pre-trained Sentence Transformer model for natural language queries.
- [Svelte](https://svelte.dev/): The frontend of this project is built with the Svelte framework.

## Contact

For any questions or feedback, please contact [Anthony Buchholz](https://github.com/yodigi7).
