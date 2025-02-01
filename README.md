Your project is an ATM simulation in Java that allows users to interact with a virtual ATM machine. The project is structured into several classes, each fulfilling a distinct role in the ATM operation.

### Overview:
1. **ATM Class**: 
   - The `ATM` class is responsible for storing the balance, deposit amount, and withdrawal amount. It has getter and setter methods to manage these values.

2. **AtmOperationImpl Class**:
   - This class implements the `AtmOperationInterf` interface and handles the main ATM operations such as:
     - **viewBalance**: Displays the available balance in the account.
     - **withdrawAmount**: Handles withdrawal requests, ensuring the amount is a multiple of 500 and that the user has sufficient balance.
     - **depositAmount**: Handles deposits and updates the balance accordingly.
     - **viewMiniStatement**: Displays a mini-statement showing all the recent transactions (both deposits and withdrawals) using a `HashMap` to store transaction history.

3. **AtmOperationInterf Interface**:
   - This interface defines the required operations that the ATM system should support: viewing balance, withdrawing funds, depositing funds, and viewing the mini statement.

4. **Main Class**:
   - The `Main` class is the entry point of the program. It simulates the user interaction with the ATM system:
     - It first verifies the ATM number and pin.
     - After authentication, the user can choose from several options like viewing balance, withdrawing money, depositing funds, and viewing the mini statement.
     - The application will continue to loop and allow users to make transactions until they choose to exit.

### Features:
- **Authentication**: Users must enter a correct ATM number and PIN to access the system.
- **Withdrawals**: Users can withdraw amounts in multiples of 500.
- **Deposits**: Users can deposit any amount, and the system updates the balance.
- **Mini Statement**: The ATM records the most recent deposit and withdrawal transactions in a mini statement for the user to view.
- **Exit Option**: Users can exit the system and "collect" their ATM card when finished.



