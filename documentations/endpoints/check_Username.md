# Endpoint
`https://thatss.me/realtime/check?type=email&value=`

# Return
✅ Avaible: `200`
❌ Unavaible: `400`
Error: `500`

# Return/json
```
{
    "status": int,
    "message": {
        "message": "string",
        "profileId": "string" || null
    }
}
```