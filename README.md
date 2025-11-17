# OPEN-SOURCE-EX-7
## NAME : Sharan Kumar G
## REG NO : 212224230260
## DEPT : AI-DS
# STEPS TO DO :
### STEP 1 : sudo pvcreate /dev/sdb
### STEP 2 : sudo vgcreate -s 8M vg_backup /dev/sdb
### STEP 3 : vgdisplay vg_backup | grep "PE Size"
### STEP 4 : PE Size               8.00 MiB
### STEP 5 : sudo lvcreate -l 50 -n lv_app_logs vg_backup
### STEP 6 : sudo mkfs.ext3 /dev/vg_backup/lv_app_logs
### STEP 7 : sudo mkdir /production \n sudo mount /dev/vg_backup/lv_app_logs /production
### STEP 8 : df -h /production
### STEP 9 : echo "/dev/vg_backup/lv_app_logs /production ext3 defaults 0 0" | sudo tee -a /etc/fstab



# OUTPUT : 

![WhatsApp Image 2025-11-12 at 14 00 04_370309a1](https://github.com/user-attachments/assets/b185b8ca-48d6-4880-bcf8-c899e634d8d0)



 # RESULT : 
 Thus the code worked correctly in the RedHat Terminal(Lab)
