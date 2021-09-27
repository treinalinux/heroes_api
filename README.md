# API Heroes

Api basic for work with heroes.

## CRUD Implemented

- Create with POST
- Read with GET
- UPDATE with PUT
- Delete with DELETE

### POST

```bash

http POST :3000/heroes name='Spider Man back home'

http POST :3000/heroes name=

```
### GET

```bash

http :3000/heroes

http :3000/heroes/20

```

### PUT

```bash

http PUT :3000/heroes/20 name='Spider Man 2'

http PUT :3000/heroes/20 name=

```

### DELETE

```bash

http DELETE :3000/heroes/21

```

## Refactor api

```bash

vim config/routes.rb
mkdir -vp app/controllers/api
mv app/controllers/heroes_controller.rb app/controllers/api/
vim app/controllers/api/heroes_controller.rb

http POST :3000/api/heroes name='Super novato'

http :3000/api/heroes

http :3000/api/heroes/19

http PUT :3000/api/heroes/23 name='Super novato 3'

http DELETE :3000/api/heroes/23

```

## Scopes Implemented

- scope search
- scope sorted_by_name

```bash

http :3000/api/heroes'?term=Machine'

http :3000/api/heroes'?term=NaoExiste'

http :3000/api/heroes

```

*Original Source:* [Paulo Eduardo Melo](#)
