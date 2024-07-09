# ZIP Password Cracker

This Python script is designed to crack passwords for ZIP files using a combination of dictionary and brute-force attacks.

## Features

1. Verify if a file is a valid ZIP archive
2. Extract contents of a ZIP file with a given password
3. Attempt to crack the password using a dictionary file
4. Generate and test passwords of a specified length

## Requirements

- Python 3.x
- pyzipper library
- zipfile library (built-in)

## Installation

1. Ensure you have Python 3.x installed on your system.
2. Ensure all required libraries are installed. You can install them using pip:
   
    ``` gitbash
      pip install -r requirements.txt
   ```

## Usage

1. Place the ZIP file you want to crack in the same directory as the script.
2. Run the script and call the appropriate function:

```python
# To verify if a file is a valid ZIP archive
print(fileHeaderReader())

# To attempt cracking with a dictionary file
password_dict("your_zip_file.zip", "your_dictionary_file.txt")

# To generate and test passwords of a specific length
generate_password("your_zip_file.zip", 4)  # 4 is the password length
