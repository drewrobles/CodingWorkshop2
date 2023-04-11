# Step 0 - Set Up Your Computer to Build Apps

Download and install the following required software if you don't already have them:
  - **Git** - [git-scm.com/downloads](https://git-scm.com/downloads)
  - **Visual Studio Code** - [code.visualstudio.com](https://code.visualstudio.com)

In a terminal window, run the following commands to download the project to your `Desktop` folder:

  ```bash
  cd ~/Desktop
  git clone https://github.com/andrewrobles/MyApp.git
  ```

- Open up the project in Visual Studio Code by going to `File > Open` and navigating to `~/Desktop/MyApp`
- Enable auto save by going to `File > Auto Save`
- Open up a terminal window by going to `View > Terminal`
---

### If you are using a Mac, run
```bash
python3 -m venv VirtualEnvironment 
```

### If you are using Windows, run
```bash
python -m venv VirtualEnvironment 
```
---
- Run the following commands:
```bash
source VirtualEnvironment/bin/activate
pip install -r requirements.txt
python manage.py migrate
```
- Now this is where the magic happens... are you ready? Run the following command:
```bash
python manage.py runserver
```
- Open the URL in a browser window provided in the terminal output - http://127.0.0.1:8000
- You should see something like this:
  ![install-worked](./screenshots/install-worked.png)

Congratulations!!! You are officially an app developer. Click on [Step 1 - Store Information In Your Database](step1.md) to continue on with your app development journey.