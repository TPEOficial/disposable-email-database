<div align="center">
  <h1>Disposable Email Database — The Largest in the World</h1>
  <h3>Access the world's largest fraud validation database for free.</h3>
  <a href="https://tpe.li/new-api-key"><img alt="16M de datos" src="https://img.shields.io/badge/16M%20data-purple?style=for-the-badge&logo=database"/></a>
  <a href="https://github.com/TPEOficial"> <img alt="GitHub" src="https://img.shields.io/badge/GitHub-purple?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="https://ko-fi.com/fjrg2007"> <img alt="Kofi" src="https://img.shields.io/badge/Ko--fi-purple?style=for-the-badge&logo=ko-fi&logoColor=white"></a>
  <br />
  <br />
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Quickstart</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://tpe.li/dsc">Discord</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/private/data-verifier">Data Verifier</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/private/email-validation">Email Validation</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/faq">FAQ</a>
  <br />
  <hr />
</div>

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
            "email": "test@test.com"
        }'
```

Or you can use...
<div align="center">
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API Node.JS SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API Bun.JS SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API Better-Auth SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API Zod SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API CLI SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API Python SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API PHP SDK</a>
  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
  <a href="https://docs.tpeoficial.com/docs/dymo-api/getting-started/quick-guide">Dymo API CURL SDK</a>
  <br />
  <hr />
</div>

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
