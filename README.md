# Description

This README file provides instructions to setup and run the API service

## Technology

- Python 3
- Django (latest version)
- Django Rest Framework (latest version)
- IDE (Preferred - VS Code)

## Basic Setup

Unzip the **mishipay_solution_tanaya.zip** folder into a directory

Navigate to that directory and perform following steps given below

## Installation

### Install Python

If python is not install on your system, refer [this link](https://www.python.org/downloads/) to install python and how to set up your system


Check if python is installed or not by typing following command in command prompt

```bash
py -V
```

### Install Django and django frameworks

Navigate to the directory where **mishipay_solution_tanaya** is located

Type the following commands in cmd to install django and its frameworks

```bash
pip install django

pip install djangorestframework
```

## Setup database

Navigate to the **mishipay_solution_tanaya** folder

```bash
cd <path>/mishipay_solution_tanaya
```

Type following commands to make migrations

```bash
python manage.py makemigrations

python manage.py migrate
```

> **Note** - If the above command does not work try using **python3** instead of **python**

# Run the app

Navigate to **mishipay_solution_tanaya** folder and type following command to run the APP

```bash
python manage.py runserver
```

> **Note** - If the above command does not work try using **python3** instead of **python**

# Access the API

You can access API from your browser or Postman

To get **Paginated API to list top users by their internet usage in last 1 Day, 7 Days and 30 Days** type

```bash
http://localhost/analytics?date=DDMMYYYY&limit=INT&page=INT
```

in your browser

To get **Users by their exact name and internet consumption usage** type

```bash
http://localhost/user/search?username=NAME_string
```
