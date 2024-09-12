
---

# **egypt-id-decode**

**egypt-id-decode** is a JavaScript library for decoding and validating Egyptian National ID numbers. It provides an easy way to extract detailed information from a 14-digit Egyptian National ID, including the birth date, gender, and governorate of issue.

## **Features**

- **ID Validation**: Checks if the provided ID number is exactly 14 digits long.
- **Detailed Parsing**: Extracts key information such as birth date, gender, governorate and etc.
- **Gender Detection**: Determines the gender based on the 13th digit of the ID.

## **Installation**

You can install the package via npm:

```bash
npm install egypt-id-decode
```

## **Usage**

Here’s a basic example of how to use the library:

```javascript
const { parseEgyptianID } = require('egypt-id-decode');

const id = '12345678901234'; // Replace with a valid 14-digit Egyptian ID
const result = parseEgyptianID(id);

if (result.error) {
    console.error(result.error);
} else {
    console.log('Birth Date:', result.birthDate);
    console.log('Governorate:', result.governorate); // Governorate where the individual was born
    console.log('Unique Number:', result.uniqueNumber);
    console.log('Check Digit:', result.checkDigit);
    console.log('Gender:', result.gender);
}
```

## **License**

This project is licensed under the MIT License. Created by Sekkena. 

---

