# FastAPI Side Hustles & Money Quotes API

## Overview
This FastAPI-based project provides two simple API endpoints:
- `/side_hustles` – Returns a random side hustle idea.
- `/money_quotes` – Returns a random money-related quote.

Both endpoints require an API key for authentication.

## Features
- Fast and lightweight API built with **FastAPI**.
- Secure API key authentication.
- Randomized responses for dynamic content delivery.

## Installation & Setup
### Prerequisites
Ensure you have **Python 3.7+** installed.

### Steps
1. **Clone the repository**:
   ```sh
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. **Create a virtual environment**:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies**:
   ```sh
   pip install fastapi uvicorn
   ```

4. **Run the API server**:
   ```sh
   uvicorn main:app --reload
   ```

## API Endpoints
### 1. Get a Random Side Hustle Idea
- **Endpoint**: `GET /side_hustles`
- **Query Parameter**: `api_key` (required)
- **Example Request**:
  ```sh
  curl "http://127.0.0.1:8000/side_hustles?api_key=123456789"
  ```
- **Example Response**:
  ```json
  {
    "side_hustle": "Freelancing - Start offering your skills online!"
  }
  ```

### 2. Get a Random Money Quote
- **Endpoint**: `GET /money_quotes`
- **Query Parameter**: `api_key` (required)
- **Example Request**:
  ```sh
  curl "http://127.0.0.1:8000/money_quotes?api_key=123456789"
  ```
- **Example Response**:
  ```json
  {
    "money_quote": "Money is a terrible master but an excellent servant. – P.T. Barnum"
  }
  ```

## Authentication
- API key is required for both endpoints.
- Example API key used: `123456789` (Change this for production use).

## Contribution
Feel free to contribute by submitting pull requests or reporting issues.

## License
This project is licensed under the MIT License.

