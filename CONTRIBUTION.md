# Contributing


## Setup

1. **Clone & Environment**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Hangman-Game.git
   python -m venv venv
   # Activate: `venv\Scripts\activate` (Win) or `source venv/bin/activate` (Mac/Linux)
   ```

2. **Dependencies**
   ```bash
   pip install -r hangman_project/requirements.txt
   ```
   *Note: This project uses `mysqlclient`. Ensure you have MySQL development headers installed if building the wheel fails.*

3. **Database**
   - The project is configured for **MySQL**.
   - Update `DATABASES` in `settings.py` with your MySQL credentials before running migrations.

4. **Run**
   ```bash
   cd hangman_project
   python manage.py migrate
   python manage.py runserver
   ```
