## ERPNext Shipping

A Shipping Integration for ERPNext with various platforms. Platforms integrated in this app are:

- [LetMeShip](https://www.letmeship.com/en/)
- [SendCloud](https://www.sendcloud.com/home-new/)

> [!TIP]
> Please make sure to get your API access enabled first, by contacting the LetMeShip support.

## Features
- Creation of shipment to a carrier service (e.g. FedEx, UPS) via LetMeShip and SendCloud. 
- Compare shipping rates. 
- Printing the shipping label is also made available within the Shipment doctype.
- Templates for the parcel dimensions.
- Shipment tracking.

## Installation

Install [on Frappe Cloud](https://frappecloud.com/marketplace/apps/shipping) or your own server:

```bash
cd ~/frappe-bench
bench get-app https://github.com/frappe/erpnext-shipping.git --branch version-14
bench --site $MY_SITE install-app erpnext_shipping
```

## Setup

Some shipping providers require the contact details of the pickup contact. Please make sure that the **User** selected as the _Pickup Contact Person_ has a first name, last name, email address, and phone number before submitting the **Shipment**.

For the 'compare shipping rates' feature to work as expected, you need to generate an API key from your service provider. Service providers have their own specific doctypes similar to those from the `Integrations`. They can be enabled or disabled depending on your needs.

![LetMeShip 2020-08-05 09-54-28](https://user-images.githubusercontent.com/17470909/89377411-500c4f80-d724-11ea-8fe5-b11fec2a5c27.png)

### Fetch Shipping Rates
![core2](https://user-images.githubusercontent.com/17470909/89377460-70d4a500-d724-11ea-8550-a2813b936651.gif)

You can see the list of shipping rates by clicking the `Fetch Shipping Rates` button. Once you picked a rate, it will create the shipment for you. 

### Shipping Label
![71bcfc9d-9d66-4a58-8238-1eeab4e9a24f 2020-08-05 09-48-32](https://user-images.githubusercontent.com/17470909/89377478-78944980-d724-11ea-8120-a5374c6e4c5e.png)

The service provider will also provide the shipping label and to generate the label, click on the `Print Shipping Label` on top of the doctype.

-----------------------
#### License

MIT
