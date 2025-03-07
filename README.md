# Devops-Travis-CI

## Project Purpose

This project is a basic app setup to demonstrate Travis CI deployment. It includes a simple application with a front-end interface, user authentication, database integration, and API endpoints. The project also includes a comprehensive CI/CD pipeline, monitoring, and logging tools.

## Project Setup

1. Clone the repository:
   ```
   git clone https://github.com/UdayDamerla5/Devops-Travis-CI.git
   cd Devops-Travis-CI
   ```

2. Install dependencies:
   - For Node.js:
     ```
     npm install
     ```
   - For Python:
     ```
     pip install -r requirements.txt
     ```

3. Start the application:
   - For Node.js:
     ```
     npm start
     ```
   - For Python:
     ```
     python main.py
     ```

## Travis CI Setup

1. Sign in to [Travis CI](https://travis-ci.com/) with your GitHub account.
2. Enable the repository in Travis CI.
3. Add the `.travis.yml` file to the root of the repository with the following content:
   ```yaml
   language: node_js
   node_js:
     - "12"
   install:
     - npm install
   script:
     - npm test
   deploy:
     provider: heroku
     api_key:
       secure: YOUR_HEROKU_API_KEY
   ```

## Running the Application

- To run the application, use the following commands:
  - For Node.js:
    ```
    npm start
    ```
  - For Python:
    ```
    python main.py
    ```

- To run tests, use the following commands:
  - For Node.js:
    ```
    npm test
    ```
  - For Python:
    ```
    pytest
    ```

## Additional Documentation

- The project includes a basic Express.js application (`app.js`) and a basic Flask application (`main.py`).
- The front-end interface is provided by `index.html`.
- Monitoring and logging configurations are available in the `monitoring/` and `logging/` directories, respectively.
