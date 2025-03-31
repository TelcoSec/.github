# TelcoSec Security Testing Tools

This directory contains security testing tools and scripts for telecommunications security research.

## Tool Categories

### Core Network Testing
- **SS7 Testing Tools**
  - [SigPloit](tools/sigploit/) - SS7/Sigtran/Diameter security testing framework
  - [SS7map](tools/ss7map/) - SS7 network mapping tool
  - [Diameter EPC Framework](tools/diameter-epc/) - Diameter protocol testing suite

### Mobile Device Security
- **Baseband Analysis**
  - [BasebandAnalyzer](tools/baseband-analyzer/) - Baseband firmware analysis toolkit
  - [RILAnalyzer](tools/ril-analyzer/) - Radio Interface Layer testing tool
  - [ModemFuzzer](tools/modem-fuzzer/) - Modem interface fuzzing framework

### SIM/eSIM Security
- **Card Testing**
  - [SIMTester](tools/sim-tester/) - SIM card security testing toolkit
  - [eSIMTools](tools/esim-tools/) - eSIM profile analysis tools
  - [APDUScanner](tools/apdu-scanner/) - APDU command testing suite

### RAN Security
- **Radio Testing**
  - [RANTester](tools/ran-tester/) - RAN security assessment toolkit
  - [AirProbe](tools/airprobe/) - Air interface analysis tools
  - [O-RANTest](tools/oran-test/) - O-RAN security testing framework

## Installation

Each tool has its own installation instructions in its respective directory. General requirements:

```bash
# Python tools
python3 -m pip install -r requirements.txt

# Docker-based tools
docker-compose up -d

# Compiled tools
make && make install
```

## Usage Guidelines

1. **Setup Environment**
   ```bash
   source setup_env.sh
   ```

2. **Configure Tools**
   ```bash
   ./configure.sh
   ```

3. **Run Security Tests**
   ```bash
   ./run_tests.sh
   ```

## Contributing

To contribute new tools or improve existing ones:

1. Fork the repository
2. Create a feature branch
3. Add your tool/improvements
4. Submit a pull request

See [Contributing Guidelines](../docs/contributing.md) for more details.

## Tool Development Standards

- Use consistent coding style
- Include comprehensive documentation
- Provide usage examples
- Include test cases
- Follow security best practices

## Security Notice

These tools are for authorized security testing only. Ensure you have proper authorization before testing any network or system.

## License

All tools are licensed under the Apache License 2.0 unless otherwise specified. 