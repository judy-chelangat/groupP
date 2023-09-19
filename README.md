# JSON Data Retrieval and Formatting

This is a simple Python script that retrieves JSON data from a specified URL, formats it for readability, and then prints the formatted JSON to the console. The code uses the `requests` library to make an HTTP GET request and the `json` library to parse and format the JSON response.

## Usage

1. **Clone the Repository**: Clone this repository to your local machine if you haven't already.

   ```shell
   git clone https://github.com/judy-chelangat/your-repo.git

2. **cd app**
3. **Install Dependencies**: If you don't have the requests library installed, you can install it using pip. <br>

   pip install requests <br>
4. **Run the Script**: Execute the Python script using the following command, <br>

python app.py

## code explanation

**Import Required Libraries:**
import requests
import json

These lines import the requests library for making HTTP requests and the json library for working with JSON data.

**Specify the URL**:


url = "https://learn-co-curriculum.github.io/json-site-example/endpoints/locations.json"

Replace this URL with the one you want to retrieve JSON data from.

**Make an HTTP GET Request:**

response = requests.get(url)

This line sends an HTTP GET request to the specified URL and stores the response in the response variable.

**Parse and Format JSON:**

json_content = json.loads(response.text)

This line parses the JSON content from the response using the json.loads() method and stores it in the json_content variable.

**Print Formatted JSON:**
print(json.dumps(json_content, indent=4, sort_keys=True))

This line formats the parsed JSON data with an indentation of 4 spaces and sorts the keys for better readability. It then prints the formatted JSON to the console.


## License

This project is licensed under the MIT License - see the LICENSE file for details.

