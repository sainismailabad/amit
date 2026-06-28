# TODO: Fix Admin Orders only showing one order

## Goal
Display **all** orders from Firebase RTDB under `orders/` and keep it realtime using `onValue()`.

## Steps
- [ ] Update `admin.js` Orders section:
  - [ ] Replace current realtime listener in `loadOrders()`
  - [ ] Use `db.ref('orders')` + `onValue()` (RTDB modular style)
  - [ ] Convert snapshot data using `Object.entries()`
  - [ ] Render via `orders.map()` (pass array to existing `renderOrders()`)
  - [ ] Show **"No Orders Found"** when empty
  - [ ] Ensure listener is not duplicated (off previous listener)
- [ ] Reload `admin.html` and verify multiple orders show + realtime updates

