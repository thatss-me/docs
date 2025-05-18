# Endpoint
`https://thatss.me/realtime/check?type=username&value=`

# Return
<br>✅ Available: `200`  
<br>❌ Unavailable: `400`  
<br>Error: `500`

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