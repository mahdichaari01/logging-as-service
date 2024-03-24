# Backend Service

The backend-gateway service is responsible for user related operations:

- user authentication
- user management
- listnes to notifications topic and relay them to the user ( TODO: Find a good mecanism to do this )
- act as a gateway to the rest of the services
- gives tokens to access ws service
- creates api keys for the user-services and his services, and expose the public key through an endpoint, keeps a list of invalid keys, notifies the kafka ( blacklist topic ) when a key is invalidated
