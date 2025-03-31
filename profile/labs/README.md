# TelcoSec Security Testing Labs

This directory contains hands-on laboratory exercises for telecommunications security testing and research.

## Lab Categories

### Core Network Security Labs
1. [SS7 Security Testing Lab](01-ss7-security/)
   - MAP message analysis
   - Location privacy testing
   - SMS/Call interception testing
   - Filtering bypass techniques

2. [Diameter Security Lab](02-diameter-security/)
   - Diameter protocol testing
   - EPC security assessment
   - Roaming security testing
   - AVP manipulation tests

3. [5G Core Security Lab](03-5g-core-security/)
   - SBA security testing
   - Network slice security
   - SEPP security assessment
   - API security testing

### Mobile Device Security Labs
1. [Baseband Security Lab](04-baseband-security/)
   - Firmware analysis
   - Protocol stack testing
   - AT command testing
   - RIL security assessment

2. [TEE Security Lab](05-tee-security/)
   - TrustZone analysis
   - Secure boot testing
   - TA security assessment
   - Crypto service testing

### RAN Security Labs
1. [RAN Security Lab](06-ran-security/)
   - Air interface testing
   - RAN protocol analysis
   - O-RAN security testing
   - Virtualization security

### SIM/eSIM Security Labs
1. [SIM Security Lab](07-sim-security/)
   - APDU testing
   - File system analysis
   - Authentication testing
   - Key extraction attempts

2. [eSIM Security Lab](08-esim-security/)
   - Profile management
   - Remote provisioning
   - LPA security testing
   - SM-DP+ integration

## Lab Environment Setup

### Requirements
- Virtual machines for core network components
- Software-defined radio hardware for RAN testing
- Smart card readers for SIM testing
- Test mobile devices
- Protocol analyzers

### Installation
```bash
# Clone lab environment
git clone https://github.com/TelcoSec/labs.git

# Setup virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Configure lab environment
./setup_lab_env.sh
```

## Lab Structure

Each lab follows this structure:
```
lab-name/
├── README.md           # Lab overview and instructions
├── setup/              # Setup scripts and configurations
├── exercises/          # Step-by-step exercises
├── tools/             # Required tools and scripts
├── solutions/         # Exercise solutions
└── documentation/     # Additional documentation
```

## Running Labs

1. **Environment Setup**
   ```bash
   cd lab-directory
   ./setup_env.sh
   ```

2. **Verify Requirements**
   ```bash
   ./check_requirements.sh
   ```

3. **Execute Lab**
   ```bash
   ./start_lab.sh
   ```

## Contributing

To contribute new labs or improve existing ones:

1. Fork the repository
2. Create a new lab directory following the structure
3. Add comprehensive documentation
4. Submit a pull request

See [Contributing Guidelines](../docs/contributing.md) for more details.

## Lab Development Guidelines

- Include clear objectives and prerequisites
- Provide step-by-step instructions
- Include expected results
- Document common issues and solutions
- Add verification steps
- Include cleanup procedures

## Security Notice

These labs are for educational purposes only. Ensure you have proper authorization before testing any network or system.

## License

All lab materials are licensed under the Apache License 2.0 unless otherwise specified. 