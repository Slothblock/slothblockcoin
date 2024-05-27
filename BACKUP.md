# SlothBlockCoin Backup Guide


Welcome to the SlothBlockCoin Backup Guide. This document will guide you through the process of backing up and restoring your SlothBlockCoin wallet. Please follow the instructions carefully to ensure the safety of your coins.



## Important Notice


The regular wallet's backup button is currently disabled due to a known issue that may cause the backup to fail during restoration. To ensure the integrity of your backup, please use the method described below.



## Backing Up Your Wallet



To create a backup of your SlothBlockCoin wallet, you will need to use the wallet's debug console. Follow these steps:



1. **Open the Wallet Debug Console:**

   - Launch your SlothBlockCoin wallet application `slothblockcoin-qt`.

   - Navigate to the `Help` menu and select `Debug Window`.

   - In the Debug Window, switch to the `Console` tab.



2. **Dump the Wallet:**

   - In the console, type the following command:

     ```
     dumpwallet "dumpfilename"
     ```

   - Replace `"dumpfilename"` with your desired filename for the backup. For example, `walletbackup.txt`.



3. **Locate the Backup File:**

   - The backup file will be saved in your data directory.

     - On **Linux**, the default directory is: `~/.slothblockcoin/backups`

     - On **Windows**, the default directory is: `%appdata%/SlothBlockCoin/backups`



## Restoring Your Wallet



To restore your wallet from a backup, you will need to import the backup file using the wallet's debug console. Follow these steps:



1. **Open the Wallet Debug Console:**

   - Launch your SlothBlockCoin wallet application.

   - Navigate to the `Help` menu and select `Debug Window`.

   - In the Debug Window, switch to the `Console` tab.



2. **Import the Wallet:**

   - In the console, type the following command:

     ```
     importwallet "fulldumpfilepath"
     ```

   - Replace `"fulldumpfilepath"` with the full path to your backup file. For example, `~/.slothblockcoin/backups/walletbackup.txt` on Linux or `C:\Users\YourUsername\AppData\Roaming\SlothBlockCoin\backups\walletbackup.txt` on Windows.



## Additional Tips



- **Regular Backups:** It is recommended to create regular backups of your wallet, especially after significant transactions.

- **Secure Storage:** Store your backup files in a secure location, such as an external hard drive or a cloud storage service with strong encryption.

- **Verify Backups:** Periodically verify that your backup files are accessible and not corrupted.



By following these instructions, you can ensure that your SlothBlockCoin wallet is safely backed up and can be restored if needed. If you encounter any issues or have further questions, please refer to the SlothBlockCoin community or support resources.



Happy Mining! 🦥💰
