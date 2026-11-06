# Social Links Profile

A responsive social links profile card built as a solution to the [Frontend Mentor Social Links Profile challenge](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ).

## Overview

This project displays a profile avatar, name, location, short bio, and a list of social media links. It focuses on clean markup, reusable data-driven rendering, and responsive styling.

### Features

- Responsive profile card for mobile and desktop layouts
- Social links rendered dynamically using Vue's `v-for`
- Keyboard-visible focus styles for links
- Local avatar image imported through Vite

## Built With

- Vue 3 (`<script setup>`)
- Vite
- CSS
- Semantic HTML

## Getting Started

### Prerequisites

Install a Node.js version compatible with the project's Vite version (Node.js 20.19+ or 22.12+).

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

### Production Build

```bash
npm run build
npm run preview
```

## Project Structure

```text
src/
├── assets/
│   └── avatar-jessica.jpeg
├── components/
│   └── SocialProfile.vue
├── App.vue
├── main.js
└── style.css
```

## What I Learned

- Rendering repeated elements from an array with Vue's `v-for`
- Importing local assets in a Vite-powered Vue application
- Building a responsive layout using CSS
- Using semantic list and anchor elements for social links

## Notes

The social links in this demo currently point to platform homepages rather than individual user profiles.

## Links

- [Frontend Mentor challenge](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ)
- **Solution URL:** Add your GitHub repository URL here
- **Live Site URL:** Add your deployed website URL here

## Acknowledgments

Design provided by [Frontend Mentor](https://www.frontendmentor.io/).