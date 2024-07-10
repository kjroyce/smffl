# smffl


## Installation

To install and run this application locally, follow these steps:

### Set Up Development Environment

#### For Flask Backend:

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/kjroyce/smffl.git
   ```

2. **Navigate to the Backend Directory**:
   ```sh
   cd backend
   ```

3. **Create and Activate a Virtual Environment** (if not already done):
   - **On Windows**:
     ```sh
     python3 -m venv venv
     venv/Scripts/activate
     ```
   
   - **On macOS/Linux**:
     ```sh
     python3 -m venv venv
     source venv/bin/activate
     ```

4. **Install Flask and Flask-CORS**:
   ```sh
   pip install Flask flask-cors
   ```

5. **Verify Flask Installation**:
   ```sh
   flask --version
   ```

#### For React Frontend:

1. **Navigate to the Frontend Directory**:
   - From the root of your project(meaning go back out to smffl using "cd .."):
     ```sh
     cd frontend
     ```

2. **Install Dependencies**:
   ```sh
   npm install
   ```

3. **Verify Installation**:
   ```sh
   npm --version
   ```

4. **Configure `package.json` Proxy**:
   - I already did this step, just check to make sure you see proxy in there.
   - Open `package.json` in the `frontend` directory.
   - Add or update the `"proxy"` key to point to your Flask backend:
     ```json
     "proxy": "http://localhost:5000"
     ```

### Development Workflow:

- The `main` branch will be used as our deployment ready branch, so don't push stuff onto it, use the `wip` branch for work. Make pull requests on github so we can test and make sure your changes work.
- The `wip` work-in-progress branch will be used as the main development branch. 
- Regularly pull updates from the `wip` branch to stay synchronized with the latest changes (`git pull origin wip`).
- Once a feature is complete, create a pull request (PR) from the feature (most likely `wip`) branch to the `main` branch on GitHub for code review and integration.
