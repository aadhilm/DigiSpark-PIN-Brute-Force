# DigiSpark PIN Brute Force Demonstration

![Arduino](https://img.shields.io/badge/Arduino-1.8%2B-blue)
![C++](https://img.shields.io/badge/C%2B%2B-11%2B-blueviolet)
![Microcontroller](https://img.shields.io/badge/Microcontroller-Digispark-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Ethical Use](https://img.shields.io/badge/Ethical%20Use-Required-red)  
![Platform](https://img.shields.io/badge/Platform-DigiSpark-9cf)  

**⚠️ Critical Disclaimer**  
This script is for **educational purposes only**. Unauthorized access to devices is illegal. Use only on devices you own or have permission to test.By using this software, you agree to use it ethically and legally.

## 🔍 Project Overview

Educational demonstration of USB HID attack vectors using DigiSpark. Shows PIN security vulnerabilities and physical device testing methodologies.
This Arduino script is designed to perform a PIN brute force attack on a device using a DigiSpark board (ATtiny85) with the DigiKeyboard library. After successfully unlocking the device, it opens a specific website in the browser.

## 🎯 Learning Objectives
✔️ Understand PIN-based security weaknesses  
✔️ Explore physical device testing methodologies  
✔️ Learn about USB HID attack vectors  
✔️ Implement defensive countermeasures  
✔️ Analyze brute-force timing patterns  
✔️ Develop security awareness against physical attacks

## 🔴 Critical Ethical Notice
- **Must comply with all applicable laws**  
- **Author not responsible for misuse**  
- **Use only on devices you own or have explicit permission to test**  
- **May trigger security lockouts on protected devices**  
- **Intended solely for ethical security research**  

### Intended Uses:
- ✅ Penetration testing with authorization  
- ✅ Security research and education  
- ✅ Digital forensics demonstrations  
- ✅ Testing your own devices' security  
- ✅ Developing defensive countermeasures  

### Forbidden Uses:
- ❌ Unauthorized access attempts  
- ❌ Malicious activities  
- ❌ Privacy violations  
- ❌ Any illegal applications  

## ⚙️ How It Works - Technical Breakdown

### Configuration Matrix
| Parameter | Default | Description | Security Impact |
|-----------|---------|-------------|-----------------|
| `start` | 0 | Starting PIN value | Lower values test common defaults |
| `endr` | 9999 | Ending PIN value | Covers 4-digit PIN space |
| `wrong_password_limit` | 3 | Attempts before delay | Mimics human error patterns |
| `wrong_password_time` | 10s | Lockout delay | Avoids security triggers |
| `auto_screen_on` | 1 | Wake screen simulation | Bypasses first auth barrier |
| `enter_key` | 1 | Auto-enter after PIN | Completes auth sequence |


## 🛠️ Hardware Requirements
- DigiSpark (ATtiny85) development board
- Micro USB cable for programming
- Target device for authorized testing

## 💾 Software Requirements
- Arduino IDE 1.8+
- DigiSpark ATtiny85 board support
- DigiKeyboard library

## ⚙️ Installation
```bash
1. Install Arduino IDE from [arduino.cc](https://www.arduino.cc/)
2. Add DigiSpark board support:
   - File > Preferences > Additional Boards Manager URLs
   - Add: `http://digistump.com/package_digistump_index.json`
   - Tools > Board > Boards Manager > Install "Digistump AVR Boards"
3. Install DigiKeyboard library
4. Upload the sketch to your DigiSpark
```

## **📜 License**  
MIT License. See [LICENSE](LICENSE).  

## **🤝Contributing ** 
Feel free to contribute to the repository by submitting issues or creating pull requests to add more tools or improve functionality.
