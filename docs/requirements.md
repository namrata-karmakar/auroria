# Requirements: what the system must do

## Functional requirements (grouped as epics)

1. Epic 1 – Product catalog

- [ ] User can view all products.
- [ ] User can filter by category (rings,
      necklaces, bracelets etc.).
- [ ] User can view product details (images,
      description, price).

2. Epic 2 – Cart & checkout

- [ ] User can add/remove items from cart. User can update quantity.
- [ ] Cart persists at least in the browser (localStorage) for now.
- [ ] User can go through a checkout form (name, address, email).
- [ ] System creates an order with order items.

3. Epic 3 – User accounts (later iteration)

- [ ] User can sign up and log in.
- [ ] Logged-in user can see their past orders.

4. Epic 4 – Admin panel (later iteration)

- [ ] Admin can create, update, deactivate products.
- [ ] Admin can view orders list.
- [ ] Admin can view dashboards/analytics.

## Non-functional requirements

1.  Performance:
    Catalog page should load in < 2s on typical connection.
2.  Security:
    Don’t leak DB credentials.
    Use basic validation and sanitization for inputs.
3.  Reliability:
    Orders are created in a single transaction (either fully created or not).
4.  Maintainability:
    Clear module boundaries in Nest (products, orders, users).
    Consistent coding style & linting.
5.  Testability:
    Core business logic unit tested (order creation, price calculations).
