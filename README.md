# Django WebSocket Chat Application

This project is a simple chat application built using Django and Django Channels. It allows users to join chat rooms and communicate in real-time using WebSockets.

## Features

- Real-time communication using WebSockets.
- Multiple chat rooms support.
- Asynchronous handling of WebSocket connections.

## Requirements

- Python 3.8+
- Django 4.0+
- Django Channels 3.0+

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/rafalwinnik0/best_chat.git
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv venv
    source venv/bin/activate
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Apply migrations:

    ```bash
    python manage.py migrate
    ```

5. We will use a channel layer that uses Redis as its backing store. To start a Redis server on port 6379:
   
    ```bash
    docker run --rm -p 6379:6379 redis:7
    ```
   
6. Run the development server:

    ```bash
    python manage.py runserver
    ```


## Running Tests

To run the unit tests, use the following command:

  ```bash
  python manage.py test chat
  ```
