* * *
- [f] *JWT bear token:
- [i] JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

- [?] *When should you use JSON Web Tokens?
- [I] Authorization: This is the most common scenario for using JWT. 
- [I] Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties

- [?] *What is the JSON Web Token structure?
- [i] ==Header.Payload.Signature==
      ==xxxxx.yyyyy.zzzzz==
	    `H: The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.
	    `P: The second part of the token is the payload, which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.
	    `S: To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

For example if you want to use the HMAC SHA256 algorithm, the signature will be created in the following way:
```
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
```

- [b] Link: https://jwt.io/introduction

Tags: #auth