Project for development M.E.R.N

# 💻 Tech Stack:
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) 


# Project Usage Manual

## Step by Step Instructions

### Step 1: Cloning the /end Repository

Make sure to clone the repository to your local machine. Open the terminal and navigate to the directory where you want to clone the repository. Then run the following command:

```bash
git clone <REPOSITORY_URL>
```
Create a folder:

```bash
mkdir server
```

After cloning, enter the server directory:

```bash
cd server
```

### Step 2: Installing Dependencies

Before starting the server, you need to install the project dependencies. Run the following command in the terminal:

```bash
npm install -g nodemon
```

This command will globally install Nodemon, a useful tool for developing Node.js applications. Then install the project dependencies:

```bash
npm install express body-parser bcrypt cors dotenv gridfs-stream multer multer-gridfs-storage helmet morgan jsonwebtoken mongoose
```

If an error occurs during installation, try deleting the `package-lock.json` and `package.json` files and running the installation command again.

### Step 3: Configuring the `package.json` File

After installing the dependencies, you need to configure the `package.json` file. Run the following command to initialize a `package.json` file:

```bash
npm init -y
```

Then open the `package.json` file and add the following code under the `"main"` key:

```json
"type": "module",
```

This is necessary due to an issue with ES6 modules. Still in the `package.json` file, add the following within the `"scripts"` key:

```json
"start": "nodemon index.js"
```

### Step 4: Creating the `.env` File

Finally, create a `.env` file following the example of the `.env.example` file provided. This file will be used to configure environment variables necessary for the server to function.

-------------------------------------------------- -----------------
## Client Installation

To get started, in your project's main folder, run the following commands:

1. Create the React application using:

     ```bash
     npx create-react-app client
     ```

2. Then enter the newly created directory:

     ```bash
     cd client
     ```

3. Install the required dependencies for the client:

     ```bash
     npm i react-redux @reduxjs/toolkit redux-persist react-dropzone dotenv formik yup react-router-dom@6 @mui/material @emotion/react @emotion/styled @mui/icons-material
     ```

Once this is done, whenever you want to start the server, make sure you start both the server and the client. You can do this by running `npm start` in the respective directories.
