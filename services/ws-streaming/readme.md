# ws-streaming Service Responsabilities

The ws-streaming service is responsible for user related operations:

- streams logs to the requesting user via websockets
- verification is done via jwt issued by the backend service
- the ws-streaming service is stateless, it relies on kafka for the replay of logs
- the ws-streaming service will serve the user until the validitity of the jwt token
