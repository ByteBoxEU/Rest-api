npm install @byteboxeu/rest-api
# oder
yarn add @byteboxeu/rest-api

javascript

import { ByteBoxClient } from '@bytebox/api';

const client = new ByteBoxClient({
  apiKey: 'IHR_API_SCHLÜSSEL',
  environment: 'sandbox' // 'production' für Live-Betrieb
});

// Rechnung erstellen
const invoice = await client.invoices.create({
  customerId: 'cust_123',
  items: [
    {
      description: 'Webdesign Leistung',
      quantity: 1,
      unitPrice: 999.00,
      taxRate: 19
    }
  ]
});

📖 Dokumentation

Vollständige API-Dokumentation, Tutorials und Code-Beispiele finden Sie in unserer offiziellen Entwickler-Dokumentation:

🔗 https://bytebox.eu/developer
