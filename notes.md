###problem1:
Failed to open a session for the virtual machine Hadoop.

WHvCapabilityCodeHypervisorPresent is FALSE! Make sure you have enabled the 'Windows Hypervisor Platform' feature. (VERR_NEM_NOT_AVAILABLE).

AMD-V is not available (VERR_SVM_NO_SVM).

Result Code: E_FAIL (0x80004005)
Component: ConsoleWrap
Interface: IConsole {872da645-4a9b-1727-bee2-5585105b9eed}
###solutation:
EDIT: Solved. Fixed by going to Start -> Settings, 
then typing "Turn Windows Features on or off".
A new window pops up containing a list of features, one of them being "Hyper-V" which was checked. 
I unchecked it, restarted my machine, now my linux OS is working again!
