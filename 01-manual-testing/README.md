<<<<<<< HEAD
# MiniMart — Manual Testing

## 1. Project Overview

**Project:** MiniMart Shopping Cart  
**Testing Type:** Manual Testing  
**Feature:** Add product to cart  
**Objective:** Verify that users cannot add products beyond the available stock.

## 2. Test Scope

The testing focuses on:
- Adding a product within the available stock.
- Preventing users from exceeding the available stock.
- Preventing users from adding out-of-stock products.

## 3. Test Cases

| Test Case ID | Test Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| TC-01 | Add a product when the cart contains 1 unit and stock is 2 | Cart quantity becomes 2 | Cart quantity becomes 2 | PASS |
| TC-02 | Add a product when the cart already contains 2 units and stock is 2 | Quantity stays at 2 and an insufficient-stock message appears | Cart quantity becomes 3 | FAIL |
| TC-03 | Add a product when stock is 0 | Product cannot be added | Product is added to the cart | FAIL |

## 4. Bug Report

### BUG-001: Cart Quantity Exceeds Available Stock

**Summary:** The cart allows users to add more products than the available stock.

**Preconditions:**
- A product has 2 units available in stock.
- The cart already contains 2 units of that product.

**Steps to Reproduce:**
1. Open the product page.
2. Set the cart quantity to 2.
3. Click the Add button again.

**Expected Result:** The cart quantity remains at 2, and the application displays an insufficient-stock message.

**Actual Result:** The cart quantity increases to 3.

**Status:** Open

## 5. Test Summary

- Total test cases: 3
- Passed: 1
- Failed: 2

**Conclusion:** The simulated application does not consistently enforce stock restrictions. The failed scenarios should be investigated and retested after the issue is fixed.

## 6. Limitations

This project uses simulated test results based on a defined scenario. The findings have not been verified against a live application.
=======
# qa-portofolio
>>>>>>> a351cac623dbc9855afcf0bf7fadd8dfb484b00f
