```
fatal: unable to access 'https://github.com/wukui-muc/Offline_RL_Active_Tracking.git/': GnuTLS recv error (-110): The TLS connection was non-properly terminated.
```
# what is the `GnuTLS`
GnuTLS is a secure communications library implementing the SSL, TLS and DTLS protocols and technologies around them. It provides a simple C language application programming interface (API) to access the secure communications protocols as well as APIs to parse and write X.509, PKCS #12, and other required structures.

The project strives to provide a secure communications back-end, simple to use and integrated with the rest of the base Linux libraries. A back-end designed to work and be secure out of the box, keeping the complexity of TLS and PKI out of application code.
# what is the `TLS`
Transport Layer Security (TLS) is a cryptographic protocol designed to provide communications security over a computer network, such as the Internet. The protocol is widely used in applications such as email, instant messaging, and voice over IP, but its use in securing HTTPS remains the most publicly visible.

The TLS protocol aims primarily to provide security, including privacy (confidentiality), integrity, and authenticity through the use of cryptography, ``such as the use of certificates, between two or more communicating computer applications.`` It runs in the presentation layer and is itself composed of two layers: the TLS record and the TLS handshake protocols.

# sovle
days agol ,in web certificates , i got github ,and add a new computer session in web session , and then ,I find that the other computers such as that using ssl to connected can not connect to the github . And when i want to clone the repositories ,I got this error: ``GnuTLS recv error (-110): The TLS connection was non-properly terminated.``<br>
so I delete the session which I add other computer.
# why cause this error?
this error is caused by the ``TLS``, city above :
```
such as the use of certificates, between two or more communicating computer applications.
```
so ,i add other computer session, so TLS can`t connect it!
