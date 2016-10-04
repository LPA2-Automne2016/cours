# Le fonctionnement 
Une API exposée au travers d'un webservice peut s'utiliser de plusieurs façon, ces facons étant du plus bas niveau au plus haut niveau.

La suite de ce cours va travailler sur une API simple : celle de Slack, au travers d'un bot d'entrée.
* Point d'entrée : https://hooks.slack.com/services/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
* Documentation de l'API : https://api.slack.com/incoming-webhooks

## Au plus bas niveau : le HTTP
On l'a vu : la majorité des webservices utilisés de nos jours sont des webservices REST, qui obéissent à des APIs simples.
Ils sont donc utilisables sans problème depuis une simple ligne de commande : 

### Démonstration depuis le shell:
```bash
curl -X POST --data-urlencode 'payload={"channel": "#general", "username": "webhookbot", "text": "This is posted to #general and comes from a bot named webhookbot."}' https://hooks.slack.com/services/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
```

### Avec [postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop) :
```
POST /services/T2B83EPCL/B2JNZ7FDM/kZwihJlEZQelW4HoT4gUem2G HTTP/1.1
Host: hooks.slack.com
Content-Type: application/json
Cache-Control: no-cache
Postman-Token: 087d9245-188a-1d20-5aa2-7cf8f97686fa

{"channel": "@sebastien", "username": "webhookbot", "text": "This is posted to #general and comes from a bot named webhookbot."}
```

### Avec Ruby ?
![reinventer la roue](http://www.hteumeuleu.fr/wp-content/uploads/2016/05/non-merci-trop-occupes.png)

**STOP ! (Rappelez vous: la morale sur l'invention et les roues ....)**

## Au niveau applicatif :

Pour quasi toutes les API publiques, il existe une Gem client qui enrobe l'API et la traduit par un simple morceau de code.
Exemple pour notre API : https://github.com/stevenosloan/slack-notifier

toutes nos lignes bas niveau se résument par :

```ruby
require 'slack-notifier'

notifier = Slack::Notifier.new "https://hooks.slack.com/services/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"
notifier.ping "Hello World"
```

## Note sur les dépendances
Lire cet article qui explique parfaitement le dilemme :
http://www.mikeperham.com/2016/02/09/kill-your-dependencies/
