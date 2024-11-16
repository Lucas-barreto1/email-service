# Email Service

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
[![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)

This project is an API built using **Java, Java Spring, AWS Simple Email Service.**


## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Lucas-barreto1/email-service.git
```

2. Install dependencies with Maven

3. Update `application.properties` puting your AWS Credentials

```yaml
aws.region=us-east-1
aws.accessKeyId= your accessKey from user
aws.secretKey=your secretKey from user
```
## Usage

1. Start the application with Maven
2. The API will be accessible at http://localhost:8080

## API Endpoints
The API provides the following endpoints:

**SEND EMAIL**
```markdown
POST /api/email - Send a e-mail from your sender to the destination
```

**BODY**
```json
{
  "to": "lucasviniciusbarreto@hotmail.com",
  "subject": "test",
  "body": "test"
}
```