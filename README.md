

---

# Global Transaction Optimizer System

This system minimizes the number of transactions among multiple banks across different regions, each utilizing various payment methods. A central World Bank, supporting all payment methods, acts as an intermediary between banks that do not share a common payment mode.

## Getting Started

Let's consider an example with the following banks:

- **World_Bank** (Central Bank)
- **First_National_Bank**
- **Union_Bank**
- **Pacific_Bank**
- **Commonwealth_Bank**
- **Morgan_Stanley**

### Example Scenario

Consider the following financial institutions:

- **Bank_of_America** (Serving as the World Bank)
- **Wells_Fargo**
- **Royal_Bank_of_Canada**
- **Westpac**
- **National_Australia_Bank**
- **Goldman_Sachs**

### Payment Transactions

Below are the transactions that need to be executed:

| Debtor Institution         | Creditor Institution       | Transaction Amount  |
|----------------------------|----------------------------|---------------------|
| **Goldman_Sachs**          | **Bank_of_America**        | Rs 100              |
| **Goldman_Sachs**          | **Wells_Fargo**            | Rs 300              |
| **Goldman_Sachs**          | **Royal_Bank_of_Canada**   | Rs 100              |
| **Goldman_Sachs**          | **Westpac**                | Rs 100              |
| **National_Australia_Bank**| **Bank_of_America**        | Rs 300              |
| **National_Australia_Bank**| **Royal_Bank_of_Canada**   | Rs 100              |
| **Bank_of_America**        | **Wells_Fargo**            | Rs 400              |
| **Wells_Fargo**            | **Royal_Bank_of_Canada**   | Rs 200              |
| **Royal_Bank_of_Canada**   | **Westpac**                | Rs 500              |

### Payment Modes

Each bank supports a specific set of payment methods, while the World Bank supports all available methods:

- **World_Bank** - Google_Pay, AliPay, Paytm
- **First_National_Bank** - Google_Pay, AliPay
- **Union_Bank** - AliPay
- **Pacific_Bank** - Google_Pay, Paytm
- **Morgan_Stanley** - Paytm
- **Commonwealth_Bank** - AliPay, Paytm

### Optimization Strategy

To optimize the transactions:

1. Calculate the net amount for each bank:
   \[
   \text{Net Amount} = [\text{Total Credits}] - [\text{Total Debits}]
   \]
2. Identify the bank with the maximum debt and the bank with the maximum credit that share a common payment method.
3. Execute the transaction using the minimum of the absolute values of the debt and credit.

Repeat the process until all debts are settled.

Thank you! Happy optimizing!

--- 

This should now be properly formatted and correctly structured for your project README.
