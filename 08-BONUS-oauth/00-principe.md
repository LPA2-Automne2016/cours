# Principe

> OAuth is an open standard for authorization, commonly used as a way for Internet users to authorize websites or applications to access their information on other websites but without giving them the passwords. This mechanism is used, for example, by Google, Facebook, Microsoft, Twitter, etc to permit the users to share information about their accounts with third party applications or websites.

>Generally, OAuth provides to clients a "secure delegated access" to server resources on behalf of a resource owner. It specifies a process for resource owners to authorize third-party access to their server resources without sharing their credentials. Designed specifically to work with Hypertext Transfer Protocol (HTTP), OAuth essentially allows access tokens to be issued to third-party clients by an authorization server, with the approval of the resource owner. The third party then uses the access token to access the protected resources hosted by the resource server.

source : https://en.wikipedia.org/wiki/OAuth

Pour résumer le principe est le suivant : il va permettre à d'autres applications
d'utiliser les données utilisateur, ainsi que d'effectuer des actions sur l'application
de départ, sans pour autant ni donner le mot de passe, ni compromettre la sécurité.

L'utilisation de base, peut se cantonner à une simple authentification.

# Schéma de fonctionnement :

![oauth](https://docs.oracle.com/cd/E39820_01/doc.11121/gateway_docs/content/images/oauth/oauth_web_server_flow.png)


Suite: [exemples d'utilisation](./01-exemples-utilisation.md)
