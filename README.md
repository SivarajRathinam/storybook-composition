# Storybook Composition Example

This repository demonstrates the use of **Storybook v8 Composition** to aggregate multiple Storybook instances into a single interface. Storybook Composition is ideal for managing stories in large-scale applications or microfrontend architectures.

## Table of Contents
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Dependencies](#dependencies)

---

## Getting Started

Follow these steps to set up and run the repository locally:

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v16 or later)
- **npm** or **yarn**

### Installation
1. Clone this repository:
   ```
   git clone https://github.com/SivarajRathinam/storybook-composition.git
   cd storybook-composition
   ```
  
2. Install dependencies:
   ```
   npm install
   # or
   yarn install
   ```
  
3. Start the Storybook:
   ```
   npm run storybook
   # or
   yarn storybook
   ```
   

### Project Structure
```
storybook-composition/
├── app1/               # First Storybook instance
├── app2/               # Second Storybook instance
├── main-storybook/     # main Storybook instance
└── README.md           # Documentation

```
### Key Files:
1. .storybook/main.js: Configures the composition and aggregates multiple Storybooks.
2. apps/app1 and apps/app2: Independent Storybooks for individual projects.

### Usage
Viewing the Composed Storybook
Run the following command to start the composed Storybook:
```
cd app1
npm run storybook

cd ../app2
npm run storybook

cd ../main-storybook
npm run storybook
```
Open http://localhost:6006 in your browser to view the composed Storybook.

### Dependencies
This repository uses the following key dependencies:

- **Storybook v8**: For building UI components.
- **React**: For the example components.
- **Webpack**: For bundling the stories.
