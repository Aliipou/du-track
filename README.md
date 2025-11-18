

# **Du-Track**

A comprehensive **Student Management System** built using **Django**, designed to manage student information, including enrollment, attendance, grades, and other administrative functionalities. This application is ideal for schools or educational institutions looking for a streamlined solution to manage student data.

**Personalized Edition** - Enhanced with modern UI/UX and customizable branding for your institution.



## **Project Structure**
```
du_track/
│
├── manage.py               # Django project manager script
├── requirements.txt        # Project dependencies
├── .env                    # Environment variables (add in .gitignore)
├── student_management/     # Main app containing settings, URLs, WSGI
├── students/               # App managing student-related functionalities
├── teachers/               # App managing teacher-related functionalities
├── classes/                # App managing class schedules and attendance
└── templates/              # HTML templates
```

## **Installation**
Follow the steps below to get the project up and running on your local machine:

### **1. Clone the Repository**
```bash
git clone https://github.com/Aliipou/du-track.git
cd du-track
```

### **2. Create a Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### **3. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **4. Set Up Database**
Make sure to set up your database (e.g., PostgreSQL) and update the `DATABASES` configuration in `student_management/settings.py`.

### **5. Run Migrations**
```bash
python manage.py migrate
```

### **6. Create Superuser**
```bash
python manage.py createsuperuser
```

### **7. Run the Application**
```bash
python manage.py runserver
```
Visit `http://localhost:8000` to access the app.

## **Configuration**
You'll need a `.env` file for environment-specific configurations. Example:

```bash
DEBUG=True
SECRET_KEY='your_secret_key'
DATABASE_URL=postgres://user:password@localhost:5432/your_db_name
```

Make sure to configure settings like database, static files, and email backend properly for production.

## **Running the Project with Docker (Optional)**
If you've Dockerized the project, you can run it as follows:

```bash
docker-compose up --build
```
This will build the Docker image and run the Django application and the PostgreSQL service.

## **Video Links**
Watch the videos to learn in proper way.
https://youtu.be/mM6vMMLYJHY


## **Testing**
You can run the unit tests with Django's built-in testing framework:

```bash
python manage.py test
```

This will run all the tests located in the `tests.py` files of your Django apps.

## **Features**
- Student enrollment and management
- Attendance tracking
- Grade management
- Teacher management
- Department organization
- Fee collection tracking
- Event and holiday management
- Library management
- Notification system
- Modern responsive UI
- Easy customization

## **Contributing**
If you want to contribute to this project, please follow the steps below:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -am 'Add a new feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Create a pull request.

## **Author**
Developed and personalized by Aliipou
Repository: https://github.com/Aliipou/du-track


