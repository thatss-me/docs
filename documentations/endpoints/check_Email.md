# Endpoint
`https://thatss.me/realtime/check?type=username&value=`

# Return
✅ Avaible: `200` \\
❌ Unavaible: `400` \\
Error: `500`

# Return/json
```
{
    "status": int,
    "message": {
        "message": "string",
        "accountId": "string" || null
    }
}
```