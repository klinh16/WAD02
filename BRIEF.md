# Brief: Implement cartTotal

**Goal**: Implement `cartTotal(items, options)` in plain JavaScript.

**Files to touch**:

- `src/cart.js` (Implementation)
- `test/cart.test.js` (Tests)

**Contract**:

- Arguments: `items` (array of `{name, price, qty}`), `options` (`{vatRate, freeShipFrom, shipFee}`).
- The output must be a **rounded number**, calculated as `subtotal + VAT + shipping`.
- Subtotal = sum of `price * qty`.
- VAT = `subtotal * vatRate`.
- Shipping = `shipFee`, unless `subtotal >= freeShipFrom` in which case it is `0`.

**Error cases & Constraints**:

- If the cart is empty (`items.length === 0`), return `0`.
- If `price` is negative, throw `RangeError`.
- If `qty` is not a positive integer, throw `RangeError`.
- **No dependencies**: Only use vanilla JavaScript (`Number.isInteger`, `Math.round`, etc.).
