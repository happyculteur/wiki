## Syntax

```
{
  "id": uuid,
  "timestamp": time,
  "firstname": string,
  "surname": string,
  "phone": integer,
  "address": [],
  "email": string,
  "interest": string,
  "level": string,
  "spaces": [],
  "has-accepted-legal-notice": boolean
}
```

## Properties

### `id`

  - Description: beekeeper's unique ID
  - Type: UUID

### `timestamp`

  - Description: timestamp for the signup
  - Type: time

### `firstname`

  - Description: the beekeeper's firstname
  - Type: string

### `surname`

  - Description: the beekeeper's surname
  - Type: string

### `phone`

  - Description: the beekeeper's phone number
  - Type: integer

### `address`

  - Description: the beekeeper physical address
  - Type: tuple of integer

### `email`

  - Description: the beekeeper's email
  - Type: string

### `interest`

  - Description: interest of the individual in Happyculteur
  - Type: List of string
  - Allowed values:
    - "training"
    - "hive"

### `level`

  - Description: experience of the individual in beekeeping
  - Type: string
    - "nothing"
    - "beginner"
    - "professional"

### `spaces`

  - Description: list of the space IDs owned by the individual. Use this to define if the individual has spaces.
  - Type: List[space_ID]

### `has-accepted-legal-notice`

  - Description: if the use rhas accepted the legal notice, must be true or the
                 user must be removed/notified
  - Type: boolean

