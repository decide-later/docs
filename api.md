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

Request:

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

Response: 

```json
{
    "success": true
}
```

or

```json
{
    "success": false,
    "errors": [
        {
            "reason": "you can not do it"
        },
        {
            "field": "name1",
            "reason": "should be filled"
        }
    ]
}
```
