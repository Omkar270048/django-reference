# django-reference

### Setup :
* Create new folder `Project`
* Open folder `Project` in `VS code`
* Create new terminal

![image](https://github.com/user-attachments/assets/f03cdfe6-2fc4-4719-b949-3b16a6507d58)

* In terminal create new `virtual machine`
```bash
python -m venv venv
```

  ![image](https://github.com/user-attachments/assets/fb207b01-5f08-463c-8134-45621b5a5734)



* activate `virtual machine`
```bash
venv/Scripts/activate
```
![image](https://github.com/user-attachments/assets/cf898574-603c-4ad0-9e4e-88118f7bac0d)

* creating new `Django project`
```bash
django-admin startproject employeeManagement
```
![image](https://github.com/user-attachments/assets/d2adc050-5975-4ee6-bedc-adaacdf0ebdc)

* Now you will see employeeManagement folder
* ![image](https://github.com/user-attachments/assets/b6cfc652-912d-46df-900d-2ef0f52e324f)

* change directory to employeeManagement:
```bash
cd employeeManagement
```
  ![image](https://github.com/user-attachments/assets/5c2644fd-ead0-48bb-b832-bd281bcc8726)

* create new app - (employeeApp)
```bash
py manage.py startapp employeeApp
```
  ![image](https://github.com/user-attachments/assets/fc366719-facb-4282-9b19-e6f9e96aa682)


* Now register your app in `settings.py`
```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'employeeApp',
]
```

* now create a folder “templates” inside folder `employeeApp`
* Now we will setup MySQL database
* Open XAMPP and make new database with name `employee`
* Open `settings.py`
* Find below code :
* ![image](https://github.com/user-attachments/assets/059f4df1-c856-4b29-b42f-c32baaf8547d)

* Make changes in it:
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'employee',
        'USER': 'root',
        'PASSWORD': '',
        'HOST':'localhost',
        'PORT':'3306',
    }
}
```


