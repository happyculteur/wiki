# Data Structure

We have to keep data organized. We splitted from now on, in three data structures:

  * beekeeper
  * individual
  * space (actualy part of individual)

## Beekeeper                                                                                                                                                                                                                                                   

### Syntax

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

### Properties

`id`
> Description: beekeeper's unique ID
> Type: UUID  

`timestamp`
> Description: timestamp for the signup
> Type: time

`firstname`
> Description: the beekeeper's firstname
> Type: string

`surname`
> Description: the beekeeper's surname 
> Type: string

`phone`
> Description: the beekeeper's phone number
> Type: integer

`address`
> Description: the beekeeper physical address
> Type: tuple of integer

`email`
> Description: the beekeeper's email
> Type: string

`seniority`
> Description: years of experience of the beekeeper
> Type: integer

`hives-number`
> Description: number of hives of the beekeeper
> Type: integer

`interest`
> Description: interest of the beekeeper in Happyculteur
> Type: List of string
> Allowed values:
>   - "training"
>   - "hive"
>   - "honey"

`is-training-billed`
> Description: if the beekeeper want his formations to be billed, false if
>              "training" is not in `interest`
> Type: boolean

`training-public`
> Description: kind of public for the beekeeper's trainings, set to null if
>              "training" not in `interest`
> Type: string
> Allowed values:
>   - "unexperienced"
>   - "beginner"
>   - "experimented"

`training-venue`
> Description: where the trainings are to happen
> Type: string
>   - "owned-hive"
>   - "happyculteur-hive"
>   - "any"
 
`has-accepted-legal-notice`
> Description: if the use rhas accepted the legal notice, must be true or the
>              user must be removed/notified
> Type: boolean



## Individual

### Syntax

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

### Properties

`id`
> Description: beekeeper's unique ID
> Type: UUID

`timestamp`
> Description: timestamp for the signup
> Type: time

`firstname`
> Description: the beekeeper's firstname
> Type: string

`surname`
> Description: the beekeeper's surname 
> Type: string

`phone`
> Description: the beekeeper's phone number
> Type: integer

`address`
> Description: the beekeeper physical address
> Type: tuple of integer

`email`
> Description: the beekeeper's email
> Type: string

`interest`
> Description: interest of the individual in Happyculteur
> Type: List of string
> Allowed values:
>   - "training"
>   - "hive"

`level`
> Description: experience of the individual in beekeeping
> Type: string
>   - "nothing"
>   - "beginner"
>   - "professional"

`spaces`
> Description: list of the space IDs owned by the individual. Use this to define if the individual has spaces.
> Type: List[space_ID]

`has-accepted-legal-notice`
> Description: if the use rhas accepted the legal notice, must be true or the
>              user must be removed/notified
> Type: boolean


## Space

### Syntax


```
{
  "id": uuid,
  "type": string,
  "size": number,
  "description": string,
  "address": []
}
```

### Properties


`id`
> Description: beekeeper's unique ID
> Type: UUID

`type`
> Description: type of space
> Type: string
> Allowed values:
>   - roof
>   - land
>   - garden
>   - terrace

`size`
> Description: the space size in square meters
> Type: integer

`description`
> Description: description of the space (by the user)
> Type: string

`address`
> Description: the space hysical address
> Type: [integer,integer]

