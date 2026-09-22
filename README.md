# JSON Data Cleaner

A simple Python project for **loading, displaying, cleaning, and saving JSON data**.

This project works with user and page data stored in a JSON file. It performs basic data cleaning operations such as removing invalid users, duplicate friends, inactive users, and duplicate pages.

## Features

* Load data from a JSON file
* Display users and pages
* Remove users without a valid name
* Remove duplicate friends
* Remove inactive users
* Remove duplicate pages
* Save cleaned data into a new JSON file

## Technologies Used

* Python
* JSON
* File Handling
* Lists
* Dictionaries
* Functions
* List Comprehension
* Set
* `json` module

## Project Structure

```text
json-data-cleaner/
│
├── json_data_cleaner.py
├── anuj1.json
├── cleared_data.json
└── README.md
```

## Input Data

The project takes data from:

```text
anuj1.json
```

The JSON file contains information about:

* Users
* User IDs
* Friends
* Liked pages
* Pages

##  Data Cleaning

The project performs the following operations:

### 1. Remove users without a name

Users whose name is missing or empty are removed.

### 2. Remove duplicate friends

Duplicate friend IDs are removed from each user's friend list.

### 3. Remove inactive users

Users who have no friends and no liked pages are removed.

### 4. Remove duplicate pages

Pages with duplicate IDs are removed so that each page ID appears only once.

##  How to Run

Make sure Python is installed on your computer.

Run the following command:

```bash
python json_data_cleaner.py
```

After execution, the cleaned data is saved in:

```text
cleared_data.json
```

##  Input

```text
anuj1.json
```

## Output

```text
cleared_data.json
```

## Example

### Input

```json
{
    "users": [
        {
            "id": 1,
            "name": "Amit",
            "friends": [2, 3],
            "liked_pages": [101]
        }
    ]
}
```

### Output

The cleaned data is stored in:

```text
cleared_data.json
```

with proper formatting and cleaned records.

## Learning Objectives

This project helps beginners understand:

* How to work with JSON files
* How to load JSON data using Python
* How to write JSON data into a file
* How to use functions
* How to use lists and dictionaries
* How list comprehension works
* How to remove duplicate values using `set`
* How to clean and prepare data before further processing

