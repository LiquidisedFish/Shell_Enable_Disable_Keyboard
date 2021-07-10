## Shell_Enable_Disable_Keyboard
When the internal laptop keyboard goes defective, this shell program can be an temp fix.

Did try the i8042 controller method using the kernel command line option: 
> *i8042.nokbd*

This would permanently disable the keyboard. 

But the best way to disable grub interaction is just to disable console for grub. It’s done by removing 'console' from available terminals for GRUB. (Debian & Ubuntu)

> /etc/default/grub
> *GRUB_TERMINAL=serial*
