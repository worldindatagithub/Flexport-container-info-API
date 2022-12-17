# Flexport Container Info API and how to work with it #
The Flexport container info API allows developers to retrieve information about cargo containers in large quantities or one at a time. Its primary purpose is to facilitate the retrieval of container details. This API can be a useful tool for those working in logistics or supply chain management.


[Container Info API](https://www.worldindata.com/api/Flexport-container-info-api)

Worldindata's API marketplace is designed to make it easier for users to access and utilize third party APIs. By presenting APIs in a user-friendly manner, our platform aims to make it simpler for developers to find and integrate the tools they need.


## Sectors, Industry, and Markets for the API ##

**Industry and Sectors**
- freight
- maritime
- logistics
- import
- export
- trade

**Client Types**
- freight and logistics companies
- importers
- exporters
- international traders




## API Parameters, JSON output and Objects ##
The GET /ocean/shipment_containers endpoint allows users to retrieve detailed information about cargo containers.

**filter parameters**
- page
- per
- f.shipment.id
- f.container_number
- f.metadata
- id


```
{
  "_object": "/api/response",
  "self": "https://api.flexport.com",
  "version": 2,
  "data": {
    "_object": "/api/collections/paginated",
    "prev": "https://api.flexport.com/ocean/shipment_containers?page=1",
    "next": "https://api.flexport.com/ocean/shipment_containers?page=3",
    "data": [
      {
        "_object": "/ocean/shipment_container",
        "metadata": {},
        "id": 283910,
        "container_type": "dry",
        "container_number": "BWSE3982156",
        "container_size": "fourty_ft",
        "seal_number": "UE_WQ2934875",
        "estimated_departure_date": "2019-02-06T19:28:25.000+00:00",
        "actual_departure_date": "2019-02-06T19:28:25.000+00:00",
        "estimated_arrival_date": "2019-02-06T19:28:25.000+00:00",
        "actual_arrival_date": "2019-02-06T19:28:25.000+00:00",
        "estimated_pickup_date": "2019-02-06T19:28:25.000+00:00",
        "actual_pickup_date": "2019-02-06T19:28:25.000+00:00",
        "estimated_delivery_date": "2019-02-06T19:28:25.000+00:00",
        "actual_delivery_date": "2019-02-06T19:28:25.000+00:00",
        "last_free_day_date": "2019-02-16T00:00:00.000Z",
        "empty_returned_date": "2019-02-28",
        "cargo_ready_date": "2019-02-06",
        "available_for_pickup_date": "2019-02-16T00:00:00.000Z",
        "estimated_available_for_pickup_date": "2019-02-16T00:00:00.000Z",
        "shipment": {
          "_object": "/api/refs/object",
          "ref_type": "/shipment",
          "link": "https://api.flexport.com/shipments/123",
          "id": 123
        },
        "container_legs": {
          "_object": "/api/refs/collection",
          "ref_type": "/ocean/shipment_container_leg",
          "link": "https://api.flexport.com/ocean/shipment_container_legs?f.shipment_container.id=123"
        },
        "items": [
          {
            "_object": "/shipment_item",
            "id": 29820,
            "total_units": 523,
            "total_weight": {
              "_object": "/quantity/weight",
              "value": 224.02,
              "unit": "kg"
            },
            "total_volume": {
              "_object": "/quantity/volume",
              "value": 8200,
              "unit": "cbm"
            },
            "purchase_order_number": "PO002811",
            "product": {
              "_object": "/product",
              "id": 84291,
              "name": "AC Adapter 12V",
              "sku": "WDVCDFD-RM00472"
            }
          }
        ]
      }
    ]
  }
}

```
**Objects**
- _object
- metadata
- id
- container_type
- container_number
- container_size
- seal_number
- estimated_departure_date
- actual_departure_date
- estimated_arrival_date
- actual_arrival_date
- estimated_pickup_date
- actual_pickup_date
- estimated_delivery_date
- actual_delivery_date
- last_free_day_date
- empty_returned_date
- cargo_ready_date
- available_for_pickup_date
- estimated_available_for_pickup_date

## SDK of the API ##

Software Development Kits (SDKs) for the Flexport cargo container details API are available in JAVA, Python, Ruby, and JavaScript. These SDKs make it easy for developers to integrate the API into their projects, regardless of the programming language they use.


### Disclaimer of representation ###
Worldindata is a platform that connects developers with data providers, and we are big fans of the Flexport container info API. However, we do not own the data that is provided through our platform. Instead, we simply strive to make the data in the world more user-friendly and accessible. Please note that the use of this data is subject to the terms and conditions of the data provider.


[Worldindata](https://www.worldindata.com)
