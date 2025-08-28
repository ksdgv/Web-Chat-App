# QuickChat Web Application

QuickChat is a real-time web chat application developed using Flask and Socket.IO. It offers an intuitive and dynamic platform where users can engage in conversations through dedicated chat rooms.

## Project Structure

```
Chat_Web_App/
    myapp/
        static/
            images/
            auth.css
            chat.css
        templates/
            auth.html
            base.html
            chat.html
        __init__.py
        config.py
        database.py
        views.py
    .gitignore
    README.md
    requirements.txt
    server.py
```

## Getting Started

1. Navigate to the project directory

   ```bash
   cd Chat_Web_App
   ```

2. Set Up a Virtual Environment

   - Create a virtual environment
     ```bash
     python -m venv venv
     ```
   - Activate the virtual environment
     ```bash
     venv\Scripts\activate  #On Windows
     ```

3. Install Dependencies

   - Install the required packages using
     ```
     pip install -r requirements.txt
     ```

4. Set Up Environment Variables

   - Create a .env File
     ```bash
     touch .env    # Navigate to your project’s root directory (Quick_Chat_App/)
     ```
   - Add Required Variables
     - Generate a Strong SECRET_KEY
       ```bash
       python -c "import secrets; print(secrets.token_hex(32))"
       ```
     - Open .env in a text editor (VS Code, Notepad, Nano, etc.) and add:
     - Add the following lines to the `.env` file:
       ```env
       SECRET_KEY=your_secret_key_here  # replace your_secret_key_here with the Secret key generated in the previous step.
       DATABASE_URL=sqlite:///database.db
       ```

5. Run the Application
   ```bash
   python server.py
   ```
6. Access the Application - Open your web browser. - Navigate to
   `html
http://localhost:5000
`
   Visit `http://localhost:5000` in your web browser to access QuickChat web application.

## Features
