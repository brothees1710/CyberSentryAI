# CyberSentryAI

## Description
CyberSentryAI is an AI-powered cybersecurity tool that analyzes security logs and identifies potential threats. It uses the Qwen AI model to classify log entries as benign, suspicious, malicious, or unknown.

## Features
- Automated security log analysis.
- Severity classification.
- Batch processing of up to 200 log entries.
- Export results in CSV and JSON formats.
- AI-generated Sigma detection rules.
- Prompt injection defense.
- Offline testing and input validation.

## Requirements
- Python 3
- Jupyter Notebook
- OpenAI Python library
- Access to a compatible AI model and API key.

## How to Run
1. Download or clone this repository.
2. Open the Jupyter notebook.
3. Install the OpenAI library using `pip install openai`.
4. Enter your API key when prompted.
5. Select your security log dataset.
6. Run the notebook cells in order.

## Results
CyberSentryAI processed 200 log entries:
- Benign: 120
- Suspicious: 71
- Malicious: 7
- Unknown: 2

## License
MIT License.
