## Syntax


```
{
  "id": uuid,
  "type": string,
  "size": number,
  "description": string,
  "address": []
}
```

## Properties


### `id`

  - Description: beekeeper's unique ID
  - Type: UUID

### `type`

  - Description: type of space
  - Type: string
  - Allowed values:
    - roof
    - land
    - garden
    - terrace

### `size`

  - Description: the space size in square meters
  - Type: integer

### `description`

  - Description: description of the space (by the user)
  - Type: string

### `address`

  - Description: the space hysical address
  - Type: [integer,integer]

