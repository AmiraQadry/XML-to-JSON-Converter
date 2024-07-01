# XML to JSON Converter
![](https://jsonformatter.org/img/xml-to-json.png)
This project provides a simple Python script to convert XML data to JSON format using the `xmltodict` and `json` libraries.

## Requirements

- Python 
- `xmltodict` library
- `json` library (included in the Python standard library)

## Installation

To install the `xmltodict` library, use the following command:

```bash
pip install xmltodict
```

## Usage

1. Clone the repository or download the script.

2. Prepare your XML data as a string.

3. Use the provided script to convert the XML string to JSON.

### Example

Here is an example of how to use the script:

```python
# Example XML string
xml_string = '''
<root>
    <person>
        <name>John Doe</name>
        <age>30</age>
        <city>New York</city>
    </person>
    <person>
        <name>Jane Doe</name>
        <age>25</age>
        <city>Los Angeles</city>
    </person>
</root>
'''

# Convert XML to JSON
json_result = xml_to_json(xml_string)

# Print the result
print(json_result)
```

### Output

The output of the above script will be:

```json
{
  "root": {
    "person": [
      {
        "name": "John Doe",
        "age": "30",
        "city": "New York"
      },
      {
        "name": "Jane Doe",
        "age": "25",
        "city": "Los Angeles"
      }
    ]
  }
}
```

## Explanation

1. **Import the required libraries:**
   The script imports the `xmltodict` and `json` libraries.

2. **Define a function to convert XML to JSON:**
   The `xml_to_json` function takes an XML string as input and returns a JSON-formatted string.

3. **Provide an XML string:**
   An example XML string is provided for demonstration purposes.

4. **Call the function with the XML string:**
   The script converts the XML string to a JSON-formatted string using the `xml_to_json` function.

5. **Print the JSON result:**
   The JSON result is printed to the console.
