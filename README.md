# Oracle HCM SOAP API Application

A prototype exploring how a web application can communicate with Oracle HCM through SOAP services. The exact requests, authentication method, and response mapping depend on the target Oracle HCM environment and its WSDL.

## Integration considerations

- Configure the WSDL endpoint for the target Oracle HCM instance.
- Use the authentication method required by that environment, such as WS-Security where applicable.
- Map SOAP responses to the application's expected data model.
- Handle service errors and timeouts explicitly.
- Keep credentials and environment-specific values out of source control.

## Local endpoints mentioned in the original project notes

- Frontend: `http://localhost:3000`
- Backend endpoint: `http://localhost:5000/api/hcm/employees`

These are documented target endpoints, not a confirmation that the application currently starts or that the Oracle integration has been tested.

## Before running

The current repository documentation does not provide a verified dependency installation or startup procedure. Check the application source and dependency manifests, configure the required environment values, and test against an authorized Oracle HCM environment before relying on the integration.

## Security

Do not commit real credentials, tokens, WSDL secrets, or customer data. Use environment variables or a local untracked configuration file, and apply the access controls required by the target environment.
