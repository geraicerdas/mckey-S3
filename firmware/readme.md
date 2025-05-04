# How to Restore McKey-S3 to Factory Firmware

## Prerequisites
- [ESP32 Flash Download Tool](https://www.espressif.com/en/support/download/other-tools)
- Factory firmware file: `McKeyS3_V4_factory.bin` (located in V2.3 folder)
- USB type C cable (connected directly to your computer)

## Step 1: Enter Programming Mode
1. Connect your device to the computer
2. Press and hold the **IO0** button
3. While holding IO0, briefly press and release the **RST** button
4. Release the **IO0** button

## Step 2: Configure Flash Tool
1. Open `flash_download_tool.exe`
2. Set parameters:
   - **Chip Type**: ESP32-S3
   - **Work Mode**: Develop
   - **Load Mode**: UART
  
    <img src="https://github.com/user-attachments/assets/5da3bfa6-075a-4e17-a3c2-6df1bd6d2751" alt="esp32 flashtool 1" width="250"/>


3. Add firmware:
   - **Binary File**: `McKeyS3_V4_factory.bin`
   - **Address**: `0x0`
     
    <img src="https://github.com/user-attachments/assets/519d6d51-ee16-45ce-8b58-83d81f2a0fcf" alt="esp32 flashtool 2" width="400"/>

4. Set communication:
   - **COM Port**: Check Device Manager (Windows)
   - **Baud Rate**: 1152000
  
    <img src="https://github.com/user-attachments/assets/41dcc194-0d53-4687-829b-b33245de4f24" alt="McKey-S3 Device Manager Programming Mode" width="800"/>


## Step 3: Flash Firmware
1. Click **START** button
2. Wait for completion (2-3 minutes):
   - Green progress bar reaches 100%
   - "FINISH" message appears
   - Verification log shows success
    
     <img src="https://github.com/user-attachments/assets/d9da7459-81bc-44c2-a143-17facc336f87" alt="esp32 flashtool 3" width="400"/>
     
<img src="https://github.com/user-attachments/assets/5ecb54dc-17d5-454f-8852-11ccd5bf0207" alt="esp32 flashtool 4" width="900"/>



## Step 4: Final Reset
1. Press **RST** button or disconnect USB cable
2. Device will reboot with factory settings

## Troubleshooting Common Issues

### Connection Failed
- Retry programming mode sequence
- Try different USB port/cable
- Check driver installation

### Flash Verification Failed
1. Confirm firmware file integrity
2. Ensure correct flash address (`0x0`)
3. Disable power-saving USB settings

### No COM Port Detected
1. Reconnect USB cable
2. Check Device Manager for unknown devices

> **Note**: Always maintain power during flashing process. Interruptions may require full chip erase.

</p>
