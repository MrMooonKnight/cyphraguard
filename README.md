# CyphraGuard 🛡️

A powerful network monitoring and system information gathering tool for managing Windows and Linux devices across your network.

## Features 🚀

- **Multi-Platform Support**: Monitor both Windows and Linux devices from a single dashboard
- **Real-Time Device Status**: Check the online/offline status of network devices
- **Comprehensive System Information**: Gather detailed information including:
  - System specifications
  - Network adapter details
  - Installed software inventory
  - Firewall configurations
  - Location information
  - And more...

- **Historical Data**: Store and view historical system information for each device
- **User-Friendly Interface**: Web-based dashboard for easy access and management
- **Secure Access**: Implements secure authentication for remote device access

## Prerequisites 📋

- Python 3.7+
- Flask web framework
- PowerShell (for Windows device management)
- SSH access (for Linux device management)
- Network connectivity to target devices
- Administrative privileges on target systems

## Installation 🔧

1. Clone the repository:
```bash
git clone https://github.com/yourusername/cyphraguard.git
cd cyphraguard
```

2. Install required Python packages:
```bash
pip install -r requirements.txt
```

3. Configure device credentials:
   - For Windows devices: Update the credentials in `getWindowsData.py`
   - For Linux devices: Ensure SSH key-based authentication is set up

## Usage 💻

1. Start the web server:
```bash
python app.py
```

2. Access the dashboard:
   - Open your web browser
   - Navigate to `http://localhost:5000`

3. Available Operations:
   - View all connected devices
   - Update client list
   - Gather system information
   - Check device status
   - View historical data
   - Monitor system changes

## Project Structure 📁

```
cyphraguard/
├── app.py              # Main Flask application
├── getWindowsData.py   # Windows device data collection
├── getLinuxData.py     # Linux device data collection
├── clientsGetter.py    # Network device discovery
├── checkStatus.py      # Device status monitoring
├── static/            # Static files (CSS, JS)
├── templates/         # HTML templates
└── Data/             # Collected system information
```

## Security Considerations 🔒

- Always use strong passwords for device access
- Implement proper network segmentation
- Regularly update system credentials
- Monitor access logs
- Use secure protocols for data transmission

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments 🙏

- Flask community for the excellent web framework
- PowerShell team for remote management capabilities
- All contributors and testers

## Support 📧

For support, please open an issue in the GitHub repository or contact the maintainers.