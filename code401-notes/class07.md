# Class 07

What is a JSON Web Token (JWT)?

- A JSON Web Token (JWT) is a compact and self-contained way to securely transmit information between parties as a JSON object. It's commonly used for authentication and authorization.

When should we use JSON Web Tokens?

- JSON Web Tokens are typically used for stateless authentication, where the server doesn't need to store session state. They are suitable for single sign-on, mobile apps, and distributed systems.

Claims are expected in which structural component of a JWT?

- Claims are expected in the payload component of a JWT. This is where information about the user or the authorization context is stored.

How is decoding the payload of a JWT considered secure?

- Decoding the payload of a JWT doesn't compromise its security because the payload is typically just base64 encoded, not encrypted. However, the integrity of the JWT is maintained through its signature, which ensures that the payload hasn't been tampered with.

What must the sender and receiver both know when sending a JWT?

- When sending a JWT, both the sender and receiver must know the secret key used to sign the token. This key is appended in the signature, ensuring that only parties with the key can validate the token's authenticity.

How can concatenated content and secret be sent and received securely to a non-technical recruiter?

- The concatenated content and secret can be shared securely with a non-technical recruiter through a secure communication channel, such as a password-protected document or a secure messaging platform. Alternatively, it can be exchanged in person or through encrypted email.

Why use JWT?

- JWTs are compact and self-contained, meaning all the necessary information is included in the token itself. This makes them easy to transmit over the network and reduces the need for server-side storage of session data.

Describe how the compact and self-contained nature of JWT is useful to a non-technical friend.

- For a non-technical friend, the compactness and self-contained nature of JWT mean that they can easily understand how the token carries all the necessary information within itself. It's like a passport that contains all your identification information in one document, making it easy to carry and present when needed.

What are the three components (the structure) of a JWT signature?

- The three components of a JWT signature are:

Header: Contains metadata about the type of token and the signing algorithm being used.
Payload: Contains claims, which are statements about the user and additional data.
Signature: Generated by encoding the header and payload along with a secret key using the specified algorithm. This signature ensures the integrity of the token and allows parties to verify its authenticity.
