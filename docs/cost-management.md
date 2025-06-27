\# Cost Management for Azure Multi-OS VM Lab



This project is designed to stay within the $100 credit limit of an Azure for Students account. Below are strategies to minimize costs:



1\. \*\*Use Free-Tier Resources\*\*:

&nbsp;  - `Standard\_B2s` VMs (750 hours/month free).

&nbsp;  - Basic SKU for public IPs and StandardSSD\_LRS for disks.



2\. \*\*Deallocate VMs When Not in Use\*\*:

&nbsp;  - Manually stop VMs via Azure Portal or run:

&nbsp;    ```powershell

&nbsp;    Stop-AzVM -ResourceGroupName MultiOSLabRG -Name <vm-name> -Force

&nbsp;    ```

&nbsp;  - Use `scripts/vm-schedule.ps1` for automated shutdown.



3\. \*\*Monitor Usage\*\*:

&nbsp;  - Check “Cost Management” in Azure Portal regularly.

&nbsp;  - Set budget alerts for $50 and $75 thresholds.



4\. \*\*Clean Up Resources\*\*:

&nbsp;  - Delete resource group after use:

&nbsp;    ```powershell

&nbsp;    Remove-AzResourceGroup -Name MultiOSLabRG -Force

&nbsp;    ```



5\. \*\*Avoid Premium Features\*\*:

&nbsp;  - Use basic Azure Monitor metrics (free) instead of Log Analytics.

&nbsp;  - Avoid premium disk types or larger VM sizes.



By following these practices, the project stays within the Azure for Students free tier and credit limits.

