# Test Cases
## Test Case 1
**Test Case Name:** Dice Dreams - in-game store - Verify that in-game store page opens and displays all items and packages correctly

**Precondition:** User has installed the application and logged in

**Steps:**  
1. Navigate to the in-game store

**Expected Result:** 
In-game store opened successfully. All items, packages, and their respective prices are displayed clearly. “Best Value” and “Most Popular” labels are visible on the relevant items.

---

## Test Case 2
**Test Case Name:** Dice Dreams - in-game store - Verify that the "Buy" button functions correctly for a specific item

**Precondition:** User has installed the application, is logged in, and has an active payment method

**Steps:**  
1. Open the in-game store
2. Tap on green button labeled "14.99$” near 220 ROLLS
3. Complete the payment process

**Expected Result:** 
The item is purchased, and the rolls are added to the user's account balance. A confirmation message appears

---

## Test Case 3
**Test Case Name:** Dice Dreams - in-game store - Buy Best Value proposition - Check that items are added to the user’s balance after purchase

**Precondition:** User has installed the application and is logged in.

**Steps:**  
1. Open the in-game store
2. Tap on green button labeled "5.99$” near Best Value proposition
3. Complete the payment process

**Expected Result:** 
The items is purchased, and added to the user's account balance. A confirmation message appears

---

## Test Case 4
**Test Case Name:** Dice Dreams - in-game store - Buy ROLLS - Check that items are added to the user’s balance after purchase

**Precondition:** User has installed the application and is logged in.

**Steps:**  
1. Open the in-game store
2. Tap on the green button labeled "14.99$” near 220 ROLLS
3. Complete the payment process
   
**Expected Result:** 
Item ROLLS are added to the user`s balance correctly

---

## Test Case 5
**Test Case Name:** Dice Dreams - in-game store - Buy COINS - Check that items are added to the user’s balance after purchase

**Precondition:** User has installed the application and is logged in.

**Steps:**  
1. Open the in-game store
2. Tap on the green button labeled "3.99$” near 220 70,000 COINS
3. Complete the payment process
   
**Expected Result:** 
Item COINS are added to the user`s balance correctly

---

## Test Case 6 
**Test Case Name:** Dice Dreams - in-game store - Buy COINS/ROLLS - Срусл that the correct amount is deducted from the bank account
**Precondition:** User has installed the application and is logged in.

**Steps:**  
1. Open the in-game store
2. Tap on the green button with price near COINS or ROLLS
3. Complete the payment process
4. Open Swagger and check the amount of payment that was deducted from the bank account (Or  OPen Postman and check with amount via GET request )
   
**Expected Result:** 
The correct amount was deducted from the bank account

---

## Test Case 7
**Test Case Name:** Dice Dreams - in-game store - Buy COINS/ROLLS - Check the message after canceling the buying

**Precondition:** User has installed the application and is logged in.

**Steps:**  
1. Open the in-game store
2. Tap on the green button with price near COINS or ROLLS
3. On Payment process click CROSS button 
   
**Expected Result:** 
Purchasing canceled and message "Purchase not completed. Something went wrong... Please try again" with OK and close(cross) buttons appeared

---

## Test Case 8
**Test Case Name:** Dice Dreams - in-game store - Check the system's response when trying to make a purchase without an internet connection

**Precondition:** User has installed the application and is logged in.

**Steps:**  
1. Open the in-game store
2. Turn off the device’s internet connection
3. Attempt to purchase any item (e.g., 70 Rolls for $5.99)

**Expected Result:** 
The message "Purchase not completed. Something went wrong... Please try again" with OK and close(cross) buttons appeared

---

## Test Case 9
**Test Case Name:** Dice Dreams - in-game store - Check that insufficient funds in the payment method prevent a purchase

**Precondition:** User has installed the application and is logged in. The user does not have enough money on bank account.

**Steps:**  
1. Open the in-game store
2. Tap on the green button with price near COINS or ROLLS
3. Complete the payment process

**Expected Result:** 
The message "Purchase not completed. Something went wrong... Please try again" with OK and close(cross) buttons appeared

---

## Test Case 10
**Test Case Name:** Dice Dreams - in-game store - Check payment process with an expired card

**Precondition:** User has installed the application and is logged in. The user has a card with expired date.

**Steps:**  
1. Open the in-game store
2. Tap on the green button with price near COINS or ROLLS
3. Complete the payment process

**Expected Result:** 
The message "Purchase not completed. Something went wrong... Please try again" with OK and close(cross) buttons appeared
