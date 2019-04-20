# API

## GET /state/current

```json
{
    "name": "in_airplane",
    "type": "regular",
    "transitions": [
        {
            "name": "jump_off",
            "title": "Открыть люк и выпрыгнуть"
        }
    ]
    "content": "Some multiline content in mixed markdown and HTML",
    "fields": [
        "name": "bla-bla",
        "type": "input",
        "validator": null
    ]
}
```

## POST /state/transit

```json
{
    "to": "state_name",
    "fields": {
        "name1": "value",
        "name2": "value",
        "name3": "value"
    }
}
```
