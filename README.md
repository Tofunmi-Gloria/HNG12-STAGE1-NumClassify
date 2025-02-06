Number Classification API

This is a simple API that takes a number and returns interesting mathematical properties about it, along with a fun fact.

Features

	•	Determines if a number is prime, perfect, or an Armstrong number.
	•	Identifies whether the number is odd or even.
	•	Calculates the sum of its digits.
	•	Fetches a fun mathematical fact about the number.
	•	Handles CORS for cross-origin requests.
	•	Returns responses in JSON format.

API Endpoint

GET /api/classify-number?number={number}

Example Request:

GET /api/classify-number?number=371

Example Response (200 OK):

{
    "number": 371,
    "is_prime": false,
    "is_perfect": false,
    "properties": ["armstrong", "odd"],
    "digit_sum": 11,
    "fun_fact": "371 is an Armstrong number because 3^3 + 7^3 + 1^3 = 371"
}

Error Response (400 Bad Request):

{
    "error": "Please provide a valid number."
}

🛠️ Installation & Setup

Prerequisites

	•	Node.js installed on your machine

Steps

	1.	Clone the repository

git clone https://github.com/Tofunmi-Gloria/HNG12-STAGE1-NumClassify.git
cd HNG12-STAGE1-NumClassify


	2.	Install dependencies

npm install


	3.	Run the server

node index.js

The API will start on http://localhost:4000 (or a different port if configured).

Deployment

This API must be publicly accessible. You can deploy it using:

	•	Render
	•	Vercel
	•	Railway
	•	Heroku
	•	AWS, Azure, or DigitalOcean

License

This project is licensed under the MIT License.

🤝 Contributing

If you’d like to contribute, feel free to fork the repo and submit a pull request!


