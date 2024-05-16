# Django Blueprint

This project serves as a starter template for Django projects, providing a baseline configuration to help you quickly set up new projects. It includes essential settings for development and production, environment variable management with `python-decouple`, and static file handling with `whitenoise`.

## Features

- Environment variable management with `python-decouple`
- Static file serving with `whitenoise`
- Example app with basic URL configuration and views
- Ready-to-use `.gitignore` and `.env.sample` files

## Setup

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Squirtled/Django-Blueprint
    cd Django-Blueprint
    ```

2. **Create a virtual environment and activate it:**
    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Copy the example environment file and configure it:**
    ```bash
    cp .env.sample .env
    ```
    Open `.env` in a text editor and replace the placeholder values with your actual configuration settings.

5. **Run the project:**
    ```bash
    python manage.py runserver
    ```

## Usage

### Environment Variables

The project uses `python-decouple` to manage environment variables. Ensure you have a `.env` file in the root directory with the necessary configuration. An example is provided in `.env.sample`.

### Static Files

Static files are managed using `whitenoise`. During development, static files are served automatically. In production, ensure you have run `python manage.py collectstatic` to collect all static files in the `staticfiles` directory.

### URL Configuration

The project includes an example app with basic URL configuration. You can add more apps and include their URLs in `base/urls.py`.

### Running Tests

To run tests, use the following command:
```bash
python manage.py test
```

### Contributing
Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

### License
This project is licensed under the MIT License - see the LICENSE file for details.