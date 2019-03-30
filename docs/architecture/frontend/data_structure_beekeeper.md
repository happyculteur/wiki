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
  "seniority": integer,
  "hives-number": integer,
  "interest": string,
  "is-training-billed": boolean,
  "training-public": string,
  "training-venue": string,
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

  - Description: the beekeeper's surnam
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

### `seniority`

  - Description: years of experience of the beekeeper
  - Type: integer

### `hives-number`

  - Description: number of hives of the beekeeper
  - Type: integer

### `interest`

  - Description: interest of the beekeeper in Happyculteur
  - Type: List of string
  - Allowed values:
    - "training"
    - "hive"
    - "honey"

### `is-training-billed`

  - Description: if the beekeeper want his formations to be billed, false if
  -              "training" is not in `interest`
  - Type: boolean

### `training-public`

  - Description: kind of public for the beekeeper's trainings, set to null if
  -              "training" not in `interest`
  - Type: string
  - Allowed values:
    - "unexperienced"
    - "beginner"
    - "experimented"

### `training-venue`

  - Description: where the trainings are to happen
  - Type: string
    - "owned-hive"
    - "happyculteur-hive"
    - "any"

### `has-accepted-legal-notice`

  - Description: if the use rhas accepted the legal notice, must be true or the
  -              user must be removed/notified
  - Type: boolean

