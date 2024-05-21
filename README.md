# BackendAssignment 


## Requirements

- Python 3.11.6
- Django 4.2.5
- Django REST Framework


## Installation

### After cloning the repository, it is advisable to create a virtual environment to ensure a clean Python installation. This can be done by running the following command:

```
python -m venv env
```

### After creating the virtual environment, it is necessary to activate it. You can find more information about this process
### You can install all the required dependencies by running the following command:

```
pip install -r requirements.txt
```


## Structure

### In a RESTful API, endpoints (URLs) define the structure of the API and specify how end users access data from our application using HTTP methods such as GET, POST, PUT, and DELETE. Endpoints should be logically organized around collections and elements, both of which represent resources in the system.

Endpoint |  HTTP Method |  CRUD Method |  Result
-- |  -- |  -- |  --
`api/vendors/` | POST | CREATE | Create a new vendor.
`api/vendors/`| GET | READ | List all vendors.
`api/vendors/{vendor_id}/`| GET | READ | Retrieve a specific vendor's details.
`api/vendors/{vendor_id}/`| PUT/PATCH | UPDATE | Update a vendor's details.
`api/vendors/{vendor_id}/`| DELETE | DELETE | Delete a vendor.
`api/purchase_orders/` | POST | CREATE | Create a purchase order.
`api/purchase_orders/`| GET | READ | List all purchase orders with an option to filter by vendor.
`api/purchase_orders/{po_id}/`| GET | READ | Retrieve details of a specific purchase order.
`api/purchase_orders/{po_id}/`| PUT/PATCH | UPDATE | Update a purchase order.
`api/purchase_orders/{po_id}/`| DELETE | DELETE | Delete a purchase order.
`api/vendors/{vendor_id}/performance/`| GET | READ | Retrieve a vendor's performance metrics.

## Use

### To test the API'S

### First, start Django's development server.

```
python manage.py runserver
```

## Commands for Vendor Profile Management:

```
Create a new vendor.
http://127.0.0.1:8000/api/vendors/

List all vendors.
http://127.0.0.1:8000/api/vendors/

Retrieve, Update and Delete a specific vendor's details.
http://127.0.0.1:8000/api/vendors/1/
```

## Purchase Order Tracking:
```
Create a purchase order.
http://127.0.0.1:8000/api/purchase_orders/

List all purchase orders with an option to filter by vendor.
http://127.0.0.1:8000/api/purchase_orders/

Retrieve, Update and Delete a specific specific purchase order details.
http://127.0.0.1:8000/api/purchase_orders/1/
```

## Vendor Performance Evaluation:
```
Retrieve a vendor's performance metrics.
http://127.0.0.1:8000/api/vendors/1/performance/
```

### This are all the total api end points for the Vendor Management System with Performance Metrics