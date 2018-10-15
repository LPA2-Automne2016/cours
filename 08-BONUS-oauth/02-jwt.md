# La gestion de l'authentification par JWT.

Json Web Token est un standard décrit dans la [RFC7519](https://tools.ietf.org/html/rfc7519).
Son schéma d'utilisation est similaire à celui de Oauthn à la différence près qu'on ne passe pas par un token qui sert à rappeler le serveur l'ayant issu.
Dans le cas du JWT, le token *est* le droit.

# Principe de fonctionnement.

Un token JWT se présente de la façon suivante :
xxxxx.yyyyyyyyyyyyy.zzzzz

Avec :
xxxx **un header** qui représente le type d'encodage utilisé par la signature du token.
Exemple :

```
{
  "alg": "HS256",
  "typ": "JWT"
}
```

Ce header est ensuite Base64URL encodé: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9`

yyyyyyy **le contenu du token**

Exemple:
```
{
  "sub": "lpa2",
  "chapitre": "authentification"
}
```

Ce contenu est lui aussi Base64URL encodé: `eyJzdWIiOiJscGEyIiwiY2hhcGl0cmUiOiJhdXRoZW50aWZpY2F0aW9uIn0`

Et pour finir le tout, header + contenu est signé à l'aide d'une clef privée et de l'algorithme mentionné dans le header, dans notre cas, HS256.

On obtient la chaine finale :
`eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJscGEyIiwiY2hhcGl0cmUiOiJhdXRoZW50aWZpY2F0aW9uIn0.3AiRk6v1X4a23KML3FeUHtfZVcRONBUdn9bgkp4SM0Y`

# Intérêt de la méthode:

Grace à la signature numérique du token, on peut être certain que :
* personne n'a modifié le contenu ou l'algorithme, sinon la signature serait invalide
* l'origine du token est connue: sans la clef privée, impossible de signer le token de façon à ce qu'il soit reconnu par la clef publique.


De plus, le format est très léger, le contenu du token est facilement vérifiable et lisible.
Pas besoin de recontacter le serveur à lorigine du token, tout est inclus

Lecture complémentaire : https://jwt.io/
