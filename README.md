# Disposable Email Database — The Largest in the World

This project provides access to the **largest and most frequently updated database of disposable email addresses** in existence.  
It is designed for developers, SaaS platforms, fraud‑prevention systems, and any service that needs to automatically detect and block temporary or throwaway email accounts.

## Key Features
- **World’s largest disposable email database** with millions of verified entries.
- **Constant real‑time updates** to ensure maximum accuracy.
- **Fast API lookup** for instant validation.
- **Lightweight and easy to integrate** into any backend or frontend workflow.
- **Perfect for fraud prevention**, user verification, spam reduction, and reputation scoring.

## Getting Started

To use the API, you simply need an **API Key**, which you can generate for free at the following link:

👉 **Create your free API Key here:**  
https://tpe.li/new-api-key

Once you have your key, you can start making requests immediately.

## Example API Request

```bash
curl -X POST https://api.tpeoficial.com/v1/private/secure/verify \
    -H "Content-Type: application/json" \
    -H "Authorization: Bearer PRIVATE_TOKEN_HERE" \
    -d '{
            "url": "https://test.com/test",
            "email": "test@test.com", 
            "phone": "+34617509462",
            "domain": "test.com",
            "creditCard": {
                "pan": "5110929780543845",
                "expirationDate": "01/2030",
                "cvv": "123"
            },
            "ip": "52.94.236.248",
            "wallet": "1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/138.0.0.0 Safari/537.36",
            "iban": "ES8101825332130207315465"
        }'
```

## Response Example

```json
{
  url: {...},
  email: {
    valid: true,
    fraud: false,
    proxiedEmail: false,
    freeSubdomain: false,
    corporate: true,
    email: "admin@lamoncloa.gob.es",
    realUser: "admin",
    didYouMean: null,
    noReply: false,
    customTLD: false,
    domain: "lamoncloa.gob.es",
    roleAccount: true,
    plugins: {...}
  },
  phone: {...},
  domain: {...},
  creditCard: {...},
  ip: {...},
  wallet: {...},
  userAgent: {...},
  iban: {...}
}                             
```

## License

This database and API are provided for security and fraud‑prevention purposes.
You may use it in commercial or personal projects according to the included license terms.

Si quieres, también puedo crear una versión más larga, más profesional, o directamente el repositorio completo (README + ejemplos + estructura).
```
