# Endpoint
`https://thatss.me/realtime/check?type=email&value=`

# Return
✅ Available: `200`  
❌ Unavailable: `400`  
⚠️ Error: `500`

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