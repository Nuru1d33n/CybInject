
# CybInject v1 (SQL Injection Practice Machine)

CybInject v1 is a penetration testing practice machine designed to help you test your SQL injection skills. This machine provides a set of vulnerable labs where you can learn, experiment, and improve your SQL injection techniques. It's a great tool for cybersecurity professionals looking to enhance their pentesting and vulnerability assessment capabilities.

### Features
- 12 SQL injection labs to test and improve your skills
- Web-based platform for simulating SQL injection attacks
- Configured with tools like Apache2 for serving vulnerable labs
- Provides a controlled environment for learning without risking actual production systems

### System Requirements
- **Virtualization Software**: VirtualBox (or any compatible virtualization software that supports OVA files)
- **OS**: Linux, macOS, or Windows
- **RAM**: Minimum of 1 GB recommended
- **CPU**: 2 cores or more
- **Disk Space**: Minimum of 2 GB

### Installation Instructions

1. **Download the OVA file**: 
   - Obtain the `CybInject.ova` file from the repository or any other source you have.
   
2. **Import the OVA file into VirtualBox**: 
   - Open VirtualBox and click on `File > Import Appliance`.
   - Select the `CybInject.ova` file from your local machine.
   - Follow the prompts to import and configure the VM.

3. **Start the Virtual Machine**:
   - Once the VM is imported successfully, start it from the VirtualBox interface.
   - The machine will automatically boot up, and you will be able to access the lab via a browser or SSH.

### Solution for Error `VERR_ACCESS_DENIED` While Opening the OVA File

If you encounter the error:
```
Error opening the OVA file 'CybInject.ova' (VERR_ACCESS_DENIED).
Result Code: E_ACCESSDENIED (0X80070005)
Component: ApplianceWrap
Interface: IAppliance {86a98347-7619-41aa-aece-b21ac5c1a7e6}
```

**Solution**: 
This error is caused due to insufficient file permissions. To fix it, you need to change the ownership of the OVA file.

Follow these steps:

1. Open the terminal.
2. Run the following command to change ownership:

   ```bash
   sudo chown your-username:your-username CybInject.ova
   ```

   Replace `your-username` with your actual username (e.g., `nurudeen`).

3. After updating the file permissions, try opening the OVA file again in VirtualBox.

This will resolve the `E_ACCESSDENIED` error, and you will be able to proceed with the import of the VM.

### Accessing the Machine

- **IP Address**: The VM is configured with a private network and can be accessed via `192.168.56.4` (can be modified based on your configuration).
- **Login Credentials**:
  - **Username**: TRY TO CRACK THIS YOURSELF
  - **Password**: TRY TO CRACK THIS YOUSELF

### Labs Included

The CybInject machine includes 12 SQL injection labs:

1. **sql1**  
2. **sql2**  
3. **sql3**  
4. **sql4**  
5. **sql5**  
6. **sql6**  
7. **sql7**  
8. **sql8**  
9. **sql9**  
10. **sql10**  
11. **sql11**  
12. **sql12**

Each lab focuses on a specific SQL injection vulnerability, allowing you to practice techniques 

### Future Developments
- **Blocking feature**: The ability to block malicious devices (in future versions).
- **Additional labs**: More labs to cover advanced SQL injection techniques.

### Contribution
Feel free to contribute to this project! If you have new SQL injection techniques, vulnerabilities, or improvements to suggest, pull requests are welcome.

### Contact
Nuruadebileje@gmail.com

### License
This project is licensed under the [MIT License](LICENSE).
