![](Pasted%20image%2020241007191825.png)
### Introduction to MERN Stack:

- **MERN** stands for **MongoDB, Express.js, React.js, and Node.js**, a powerful full-stack JavaScript framework.
- It enables developers to build modern web applications efficiently by using JavaScript for both front-end and back-end development.

### Components of the MERN Stack:

1. **MongoDB**:
    
    - NoSQL database where the application's data is stored.
    - It stores data in flexible, JSON-like documents, which is ideal for applications requiring fast iterations and scalability.
2. **Express.js**:
    
    - A lightweight web application framework for Node.js that provides a robust set of features to build single-page, multi-page, and hybrid web applications.
    - It simplifies the server-side development process.
3. **React.js**:
    
    - A front-end JavaScript library for building user interfaces, particularly single-page applications (SPAs).
    - It allows developers to create reusable UI components and manage the view layer of the web app.
    - Awesome React Render : https://github.com/chentsulin/awesome-react-renderer
    - [[Famous Web-apps]] used by ReactJS 
      
4. **Node.js**:
    
    - A server-side JavaScript runtime built on Chrome's V8 engine.
    - It enables developers to build scalable, high-performance web servers that can handle a large number of simultaneous requests.
    

**List of JavaScript Engines:**

| **Browser**              | **Name of Javascript Engine** |
| ------------------------ | ----------------------------- |
| Google Chrome            | V8                            |
| Edge (Internet Explorer) | Chakra                        |
| Mozilla Firefox          | Spider Monkey                 |
| Safari                   | Javascript Core Webkit        |

### Benefits of MERN Stack:

- **Full JavaScript Stack**: Both the front-end and back-end are handled using JavaScript, simplifying development.
- **Scalability**: MongoDB is highly scalable, making it suitable for large-scale applications.
- **React.js**: Provides an interactive and responsive user experience with reusable components.
- **Efficient Development**: By using tools like **npm**, MERN developers have access to a vast ecosystem of libraries and modules. (https://www.npmjs.com/)

### MERN Vs MEAN
![](Pasted%20image%2020241007203559.png)

### MERN + Devops = Fullstack Developer

#### DevOps : 

- **Continuous Integration (CI)**
- **Continuous Deployment (CD)**
- **Automation**
- **Monitoring and Logging**

### Tools
#### 1. **Git**:

- **Definition**: Git is a distributed version control system that tracks changes in the source code during software development.
- **Importance**: It helps developers collaborate on projects, track different versions of code, and revert back to earlier versions if needed.
- **Usage**:
    - You can initialize a repository using `git init`, track changes using `git add` and `git commit`, and collaborate with others using `git push` and `git pull`.
- **Key Features**:
    - **Branching**: Allows you to work on new features or bug fixes independently without affecting the main codebase.
    - **Merging**: Combine different branches once development is completed.

#### 2. **Visual Studio Code (VS Code)**:

- **Definition**: VS Code is a lightweight yet powerful source code editor developed by Microsoft. It supports debugging, task running, version control, and more.
- **Importance**: It's widely used due to its ease of use, customizability, and rich extensions marketplace.
- **Usage**:
    - Install VS Code, and you can start writing and editing your JavaScript/Node.js code with ease. It also integrates seamlessly with Git.
- **Key Features**:
    - **IntelliSense**: Provides smart code completions based on variable types and function definitions.
    - **Extensions**: Enhances productivity with plugins for various programming languages, linters, and themes.

#### 3. **Node.JS**:

- **Definition**: Node.js is a JavaScript runtime built on Chrome's V8 engine that allows developers to run JavaScript on the server.
- **Importance**: It enables full-stack development using a single language, JavaScript.
- **Usage**:
    - Install Node.js, and you can run server-side scripts using commands like `node server.js`. It also includes npm (Node Package Manager), which is used to install libraries.
- **Key Features**:
    - **Non-blocking I/O**: Handles asynchronous operations efficiently, which is ideal for scalable web applications.
    - **NPM**: Offers a vast ecosystem of open-source libraries that speed up development.

#### 4. **MongoDB Atlas**:

- **Definition**: MongoDB Atlas is a cloud-based NoSQL database as a service that makes it easy to set up, operate, and scale MongoDB databases.
- **Importance**: As a managed service, Atlas allows developers to focus on building applications rather than managing infrastructure.
- **Usage**:
    - You can create a new database cluster in Atlas, connect it to your Node.js app using MongoDB’s driver, and manage it via a web UI.
- **Key Features**:
    - **Automatic Scaling**: Atlas automatically adjusts the database size based on demand.
    - **Security**: Includes built-in security features like encryption and access control.
#### 5. **MongoDB Compass**:

**MongoDB Compass** is a graphical user interface (GUI) for MongoDB that provides a visual interface to explore, manipulate, and analyze your MongoDB data. It’s particularly useful for developers and database administrators who prefer an easy-to-use interface over command-line tools.
#### 6. **Create React App**:

- **Definition**: Create React App (CRA) is a command-line tool to quickly set up a new React project with no configuration needed.
- **Importance**: It eliminates the hassle of setting up and configuring a React project from scratch, allowing developers to focus on building the application.
- **Usage**:
    - Install Create React App using the command `npx create-react-app my-app`. This will generate a basic folder structure and set up the project with all necessary dependencies.
- **Key Features**:
    - **Zero Configuration**: Out-of-the-box build scripts, development server, and optimizations for React applications.
    - **Live Reload**: Automatically reloads the application when you make changes to the code.

#### 7. **CodeSandbox**:

- **Definition**: CodeSandbox is an online IDE that enables developers to build, share, and collaborate on web development projects in a browser.
- **Importance**: It's ideal for quick prototyping and testing of ideas without needing to install any local tools.
- **Usage**:
    - Go to CodeSandbox.io, and you can start building a MERN stack project or any other web application by choosing from the various templates (like React, Node.js, etc.).
- **Key Features**:
    - **Real-time Collaboration**: Multiple developers can work on the same project simultaneously.
    - **Pre-built Templates**: Start coding immediately using pre-configured templates for various frameworks (e.g., React, Vue, Angular).

#### **8.Postman**: A Web API Testing Tool:

**Postman** is a powerful and widely-used tool for **API development** and testing. It simplifies the process of sending HTTP requests and testing RESTful APIs. Postman provides a user-friendly interface that allows developers to make requests, analyze responses, and organize API workflows efficiently.

# Build Application
### 1. [[Create Database to Atals]]
### 2. Create React App

```
npm install -g create-react-app
```

```
npx create-react-app react-user-management
```

### 3. Create New Repo on Github

(App name and Repo name should be same)

```
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin <RepoLink>
git push -u origin main

```

###### Enter the Github Credential 

# ------(Learn [[JSX and Components]]  )-----

### 4. Install Material UI

```
npm install @mui/material @emotion/react @emotion/styled
```

### 5. React Router Dom

```
npm i react-router-dom

```

Optional
```
npm install --save-dev ajv@^7 
```

# ------(Learn Folder Structure, Material UI, Routing,)-----

### 6.  [[Start Build Navbar]], Routes, Pages 


# ----- (Learn [[UseState]]) ---- 
# ----- (Learn [[Virtual Dom]]) -----

Register and Login form

---- Front end Design is done  and push the Changes------

### 7. Connect Atlas Database to Compass)

mongodb+srv://wissenskill:hOODUfqG4BZO49Ct@usermanagement.glmti.mongodb.net/myapp?retryWrites=true&w=majority&appName=UserManagement

