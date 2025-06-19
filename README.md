# coding-dashboard
This is a personal web application designed to help you organize and manage your learning resources across various programming languages, machine learning/AI topics, Data Structures and Algorithms (DSA), practice websites, and personal projects. It features a modern, interactive design and uses browser's Local Storage for data persistence.

Features
Multi-Tab Organization: Navigate between main categories like "Languages", "Practice", "ML/AI", "DSA", "Projects", and "Additional Resources".

Sub-Category Filtering: "Languages" and "ML/AI" tabs include sub-categories (e.g., Python, JavaScript, TensorFlow, NLP) to further refine your resource lists.

Resource Management (CRUD):

Add New: Easily add new resources with a name, link (URL), optional category, and notes.

Edit: Modify existing resource details.

Delete: Remove resources you no longer need.

Local Storage Persistence: All your added resources are automatically saved in your browser's local storage, so they remain available even if you close and reopen the application.

Responsive Design: The application is styled to be visually appealing and functional across various devices (desktop, tablet, mobile).

Dynamic UI: Includes modern CSS for smooth transitions, hover effects, and animations to provide a "dashing" and engaging user experience.

Getting Started
Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

Prerequisites
You need to have Node.js and npm (Node Package Manager) installed on your system.

Node.js: Download & Install Node.js (npm is included with Node.js)

Installation
Clone the repository:

git clone <your-repository-url>
cd <your-repository-name>

(Replace <your-repository-url> and <your-repository-name> with your actual repository details)

Navigate into the project directory:
If you've cloned it directly into a parent folder, you might need to cd my-react-app if the React app was created in a sub-directory.

Install dependencies:

npm install

Running the Application
To run the application in development mode:

npm start

This command runs the app in development mode. Open http://localhost:3000 to view it in your browser. The page will reload if you make edits. You will also see any lint errors in the console.

Deployment to GitHub Pages
This application is configured for easy deployment to GitHub Pages using the gh-pages package.

Ensure homepage is set in package.json:
Open your package.json file and make sure the homepage property is set correctly to your GitHub Pages URL:

"homepage": "https://<YOUR_GITHUB_USERNAME>.github.io/<YOUR_REPOSITORY_NAME>",

Replace <YOUR_GITHUB_USERNAME> and <YOUR_REPOSITORY_NAME> with your actual GitHub username and repository name.

Install gh-pages (if not already installed):

npm install --save-dev gh-pages

Add predeploy and deploy scripts to package.json:
Ensure these scripts are present in your package.json under the "scripts" section:

"scripts": {
  "start": "react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test",
  "eject": "react-scripts eject",
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
},

Deploy your application:
Run the deploy script from your terminal:

npm run deploy

This command will build your React application for production and then push the compiled files to a gh-pages branch in your repository.

Configure GitHub Pages in your repository settings:

Go to your GitHub repository in your web browser.

Click on "Settings".

In the left sidebar, click on "Pages".

Under "Source," select the branch gh-pages and keep the folder as / (root).

Click "Save".

Your site should be published at the homepage URL specified in your package.json within a few minutes. If you don't see the changes immediately, try a hard refresh in your browser (Ctrl + F5 or Cmd + Shift + R).

Technologies Used
React: A JavaScript library for building user interfaces.

CSS: For styling and layout.

Local Storage: For client-side data persistence.

gh-pages: npm package for deploying to GitHub Pages.

Google Fonts: Inter and Roboto Mono for typography.
