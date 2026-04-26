---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
---

# Liquidation Process

### **Specific Flow of Liquidation**

1. **Occurrence of Insufficient Collateral**:
   * When a borrower has assets as collateral in the punodwoɔ protocol and has borrowed other assets, market price fluctuations may cause the collateral to no longer cover the borrow amount.
   * When the borrower's base asset borrows reach or exceed the liquidation threshold, according to protocol rules,\
     that position becomes eligible for liquidation.
2. **Triggering the Liquidation Process**:
   * Anyone can liquidate positions eligible for liquidation. Mainly traders and bots discover positions eligible for liquidation and execute liquidation.
3. **Repayment of Borrow Amount**:
   * The borrower's debt is repaid using the protocol's base asset reserves.\
     If reserves are insufficient, liquidators use flash loans, etc., to repay.\
     This completes the borrower's borrow position and removes it from liquidation eligibility.
4. **Confiscation of Collateral**:
   * As part of liquidation, the borrower's collateral is confiscated. The amount of collateral confiscated is calculated by adding\
     the "liquidation penalty" on top of the borrow amount.
   * The remainder after subtracting the borrow amount and liquidation penalty from the collateral is returned to the borrower.
5. **Distribution of Liquidation Penalty**:
   * Of the confiscated collateral, the "liquidation penalty" portion is split between the protocol and the liquidator.\
     Part of the penalty goes to the protocol's reserves, and another part becomes the liquidator's profit.
6. **Sale of Collateral**:
   * When confiscated collateral is transferred to the protocol, the protocol's reserves are checked.\
     Only when the protocol's reserves do not meet the target reserves (target reserve amount),\
     that collateral is sold at a discount.

### Design Philosophy of Liquidation

In this way, the liquidation process is designed to maintain protocol stability and liquidity, minimize borrower losses,

and provide appropriate incentives to liquidators.
