
# Pokedex


## Description

This is a simple pokedex app that allows you to search for pokemon and view their details. It also allows you to add pokemon to your favorites list and view them later.

## API and Data Sample
https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/

https://pokeapi.co/api/v2/pokemon/?limit={limit}

## Pages 

register.html - The sign up page, allows the user to create an account.

login.html - Allows the user to login.

detail.html - A page to view view the individual pokemon and their details

index.html - The home page, displays all pokemon






#### Get single pokemon: https://localhost:8000/api/pokemon/1/

```json
{
    "pokemon": {
        "id": 1,
        "name": "bulbasaur",
        "number": 1,
        "height": 7,
        "weight": 69,
        "image_url": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/1.png",
        "types": [
            {
                "id": 47,
                "name": "grass"
            },
            {
                "id": 48,
                "name": "poison"
            }
            ], 
        "abilities": [
            {
                "id": 252,
                "name": "overgrow",
                "effect": "Strengthens grass moves to inflict 1.5\u00d7 damage at 1/3 max HP or less."
            },
            {
                "id": 253,
                "name": "chlorophyll",
                "effect": "Doubles Speed during strong sunlight."
            }
        ]
    }
}
```

#### Get all pokemon: https://localhost:8000/api/pokemon/

```json
{
    "pokemon": [
        {
            "id": 1,
            "name": "bulbasaur",
            "number": 1,
            "height": 7,
            "weight": 69,
            "image_url": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/1.png",
            "types": [
                {
                    "id": 47,
                    "name": "grass"
                },
                {
                    "id": 48,
                    "name": "poison"
                }
            ],
            "abilities": [
                {
                    "id": 252,
                    "name": "overgrow",
                    "effect": "Strengthens grass moves to inflict 1.5\u00d7 damage at 1/3 max HP or less."
                },
                {
                    "id": 253,
                    "name": "chlorophyll",
                    "effect": "Doubles Speed during strong sunlight."
                }
            ]
        },
        {
            "id": 2,
            "name": "ivysaur",
            "number": 2,
            "height": 10,
            "weight": 130,
            "image_url": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/2.png",
            "types": [
                {
                    "id": 47,
                    "name": "grass"
                },
                {
                    "id": 48,
                    "name": "poison"
                }
            ],
            "abilities": [
                {
                    "id": 252,
                    "name": "overgrow",
                    "effect": "Strengthens grass moves to inflict 1.5\u00d7 damage at 1/3 max HP or less."
                },
                {
                    "id": 253,
                    "name": "chlorophyll",
                    "effect": "Doubles Speed during strong sunlight."
                }
            ]
        },
        {
            "id": 3,
            "name": "venusaur",
            "number": 3,
            "height": 20,
            "weight": 1000,
            "image_url": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/3.png",
            "types": [
                {
                    "id": 47,
                    "name": "grass"
                },
                {
                    "id"
```

#### Get pokemon from search term: https://localhost:8000/api/pokemon/?q=bulbasaur

```json
{
    "pokemon": [
        {
            "id": 1,
            "name": "bulbasaur",
            "number": 1,
            "height": 7,
            "weight": 69,
            "image_url": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/1.png",
            "types": [
                {
                    "id": 47,
                    "name": "grass"
                },
                {
                    "id": 48,
                    "name": "poison"
                }
            ],
            "abilities": [
                {
                    "id": 252,
                    "name": "overgrow",
                    "effect": "Strengthens grass moves to inflict 1.5\u00d7 damage at 1/3 max HP or less."
                },
                {
                    "id": 253,
                    "name": "chlorophyll",
                    "effect": "Doubles Speed during strong sunlight."
                }
            ]
        }
    ]
}
```