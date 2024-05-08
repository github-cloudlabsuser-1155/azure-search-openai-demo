# Backend Application

This is the backend part of the Azure Search OpenAI Demo application. It is written in Python and uses Quart as the web framework.

## Getting Started

To start the backend application, navigate to the `app` directory and run the start script:

```sh
cd app
./start.sh
```

## API Endpoints

The backend provides several API endpoints:

- `/chat`: Handles chat requests.
- `/auth_setup`: Sends MSAL.js settings to the client UI.
- `/config`: Returns the configuration.
- `/upload`: Handles file uploads.
- `/delete_uploaded`: Deletes uploaded files.
- `/list_uploaded`: Lists uploaded files.

## Authentication

The application uses the `authenticated` decorator to protect certain routes. The authentication process is handled by Azure Active Directory.

## Environment Variables

The application uses several environment variables for configuration. Please refer to the `config.py` file for more details.

# Backend Requirements

The backend application requires the following Python packages:

```
aiofiles==23.2.1
aiohttp==3.9.3
aiosignal==1.3.1
annotated-types==0.6.0
anyio==4.3.0
asgiref==3.7.2
attrs==23.2.0
azure-ai-documentintelligence==1.0.0b2
azure-common==1.1.28
azure-core==1.30.1
```

These packages are listed in the `requirements.txt` file and can be installed using pip:

```sh
pip install -r requirements.txt
```


## Contributing

Contributions are welcome. Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)


The backend application uses the following third-party libraries:

- [Quart](https://pgjones.gitlab.io/quart/)
- [Pydantic](https://pydantic-docs.helpmanual.io/)
- [Azure SDK for Python](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview)