# requests-iam-session

Python requests library implemented with build-in AIM authentication, using current credentials

## Installation

Add custom pypi repository to `pyproject.toml` file

```
[[tool.poetry.source]]
url = "https://pypi.fury.io/epsy/"
name = "fury"
```

Install package

```
poetry add requests-iam-session
```

## Usage example

```python
from requests_iam_session import AWSSession

session = AWSSession("https://rest.epsy.in/")
response = session.get("/users/04c3480d-72e3-4d16-919e-2c71858fc258")

print(response.json())
```
