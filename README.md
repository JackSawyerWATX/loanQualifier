# Loan Qualifier

A small JavaScript demonstration that checks annual income and credit score against minimum requirements for duplex, condo, and car loans.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Security](#security)
- [How to Contribute?](#how-to-contribute)
- [What's Next?](#whats-next)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Author](#author)

## About

Loan Qualifier is a command-line example of basic loan eligibility checks. It evaluates a sample applicant's annual income and credit score, then reports which loan types meet the configured minimums. It is an educational example, not a financial or lending decision service.

## Features

- Checks eligibility for duplex, condo, and car loans.
- Applies income and credit score minimums to each loan type.
- Prints example results for four sample applicants.

## Tech Stack

- JavaScript (Node.js)

## Architecture

The application is a single JavaScript file. It defines loan eligibility thresholds, evaluates income and credit score in `getLoanMessage`, and logs results for a set of sample applicants. There are no external services or dependencies.

## Project Structure

```text
loanQualifier/
└── script.js    # Loan eligibility rules and sample runs
```

## Getting Started

### Prerequisites

- Node.js installed on your machine.

### Run the example

From the project directory, run:

```bash
node script.js
```

The script prints the eligibility result for each sample applicant to the console.

## Configuration

The minimum income and credit score requirements are constants at the top of `script.js`:

| Loan type | Minimum annual income | Minimum credit score |
|---|---:|---:|
| Duplex | $60,000 | 700 |
| Condo | $45,000 | 680 |
| Car | $30,000 | 650 |

To try different applicants, change the sample values passed to `getLoanMessage` near the end of the file. The current values and thresholds are illustrative and are not financial advice.

## Security

This example runs locally and does not collect, store, or transmit personal or financial data. Do not use it to make real lending decisions: it has no input validation, underwriting logic, privacy controls, or regulatory review.

## How to Contribute?

Contributions are welcome. You can help by improving the eligibility examples, adding tests, or clarifying the documentation.

1. Fork the repository and create a branch for your change.
2. Make a focused update.
3. Run `node script.js` to check the example still runs.
4. Open a pull request describing the change.

## What's Next?

- Accept applicant details as command-line input.
- Add input validation and automated tests.
- Separate eligibility rules from sample data.
- Document loan assumptions and configurable requirements.

## License

No license is currently specified. Until a license is added to the repository, reuse and redistribution permissions are not defined.

## Acknowledgements

Thanks to the maintainers and contributors who help improve this project.

## Author

Jack Sawyer
