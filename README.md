# PoetryDB API Test Cases

This repository contains detailed test cases for testing the PoetryDB API, which offers endpoints to retrieve poetry data in various forms.

## Test Cases

| Test Case ID | Description                        | API Endpoint                        | Expected Result                                         | Validation Method                             |
|--------------|------------------------------------|-------------------------------------|---------------------------------------------------------|-----------------------------------------------|
| **TC01**     | Retrieve poems by exact author name| `/author/Percy%20Bysshe%20Shelley:abs` | JSON array of Percy Bysshe Shelley's poems           | Check JSON for correct author and poem details|
| **TC02**     | Retrieve specific poem by title    | `/title/Ozymandias`                 | JSON object containing the poem "Ozymandias" details    | Validate JSON matches known poem details      |

## Validation Description

Each response from the PoetryDB API is validated by checking:
- **Correctness of the data**: Ensuring that the data in the JSON response matches expected values based on known literary sources.
- **Data format**: Confirming that the data is returned in a proper JSON format and contains all expected keys (e.g., `title`, `author`, `lines`).
- **Response status**: Verifying that the API returns a **200** OK status, indicating successful retrieval of data.

The validation ensures that the API behaves as expected under different conditions and that the data integrity is maintained.
