# requests-iam-session

Python requests library implemented with build-in AIM authentication, using current credentials

## Installation

Add custom pypi repository to `pyproject.toml` file

```
[[tool.poetry.source]]
url = "***REMOVED***"
name = "fury"
```

Install package

```
poetry add requests-iam-session
```

## Usage example

```python
from requests_iam_session import AWSSession

session = AWSSession("https://***REMOVED******REMOVED***/")
response = session.get("/users/***REMOVED***")

print(response.json())
```
