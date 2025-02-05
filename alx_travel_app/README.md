# API Endpoints Documentation

## Listings
- `GET /api/listings/`: List all available travel listings
- `POST /api/listings/`: Create new listing (requires authentication)
- `GET /api/listings/{id}/`: Retrieve specific listing details
- `PUT /api/listings/{id}/`: Update listing (owner only)
- `DELETE /api/listings/{id}/`: Delete listing (owner only)

## Bookings
- `GET /api/bookings/`: List user's bookings (requires authentication)
- `POST /api/listings/`: Create new listing (requires authentication)
- `GET /api/listings/{id}/`: Retrieve specific listing details
- `PUT /api/listings/{id}/`: Update listing (owner only)
- `DELETE /api/listings/{id}/`: Delete listing (owner only)

## Testing the API
1. **Starting development server:**
```
python manage.py runserver
```

2. **Access API documentation:**
[](http://localhost:8000/swagger/)

3. **Example request using curl:**
```
curl http://localhost:8000/api/listings/

curl -X POST -H "Content-Type: application/json" -H "Authorization: Token <your-token>" -d '{
    "title": "Beach House",
    "description": "Oceanfront property",
    "price_per_night": 250.00,
    "location": "Miami, FL"
}' http://localhost:8000/api/listings/
```
