# T117-PS-043: Metro Fare and Smart Card Engine

## 1. Project Overview

The Metro Fare and Smart Card Engine is a Python-based application that simulates metro smart card operations.

The application processes passenger entry and exit events, calculates journey fares based on travel zones and time, manages smart card balances, applies penalties, and generates journey, balance, and revenue reports.

**Project ID:** T117-PS-043

**Project Title:** Metro Fare and Smart Card Engine with Zone Fares, Peak Pricing and Penalties

## 2. Features

- Zone-based fare calculation.
- Peak-hour and off-peak pricing.
- Smart card fare discounts.
- Student and senior citizen concessions.
- City supplement calculation.
- Smart card balance management.
- Card top-up and refund operations.
- Tourist pass purchase and validity management.
- Tap-in and tap-out event processing.
- Mismatch and overstay penalties.
- Daily fare cap for standard cards.
- Automatic card balance reload.
- CSV-based input and output reports.
- Automated testing using pytest.

## 3. Technologies Used

- Python
- CSV file handling
- Decimal arithmetic
- Dataclasses
- Pytest
- Visual Studio Code

## 4. Project Structure

```text
metrofare/
|
|-- main.py
|-- models.py
|-- fareengine.py
|-- event_processor.py
|-- card_service.py
|-- loader.py
|-- reports.py
|-- README.md
|-- requirements.txt
|-- .gitignore
|-- design_document.pdf
|-- decision_log.md
|
|-- data/
|   |-- stations.csv
|   |-- cards.csv
|   |-- events.csv
|   |-- holidays.csv
|
|-- output/
|   |-- journey_history.csv
|   |-- card_balances.csv
|   |-- revenue.csv
|
|-- tests/
    |-- __init__.py
    |-- test_station.py
    |-- test_card.py
    |-- test_fare.py
    |-- test_event_processor.py
    |-- test_card_service.py
    |-- test_reports.py
    |-- test_tourist_pass.py
|
|-- docs/
|-- source/
```

## 5. Requirements

- Python 3.10 or later
- pip
- pytest

Install the required testing dependency using:

```powershell
python -m pip install -r requirements.txt
```

## 6. Setup Instructions

### Step 1: Clone the repository

```powershell
git clone https://github.com/varshinis108-ai/T117-PS-043.git
cd T117-PS-043
```

### Step 2: Create a virtual environment

```powershell
python -m venv .venv
```

### Step 3: Activate the virtual environment

For Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### Step 4: Install dependencies

```powershell
python -m pip install -r requirements.txt
```

## 7. Running the Application

Run the following command from the project root directory:

```powershell
python main.py
```

The application:

1. Loads station information.
2. Loads smart card information.
3. Loads holiday information.
4. Loads metro events.
5. Processes passenger tap-in and tap-out events.
6. Calculates journey fares and penalties.
7. Updates smart card balances.
8. Generates CSV reports.

## 8. Fare Calculation

The fare engine considers:

- Number of zones crossed.
- Student and senior citizen concessions.
- Smart card discounts.
- Peak-hour fare adjustments.
- Off-peak fare adjustments.
- City supplement.

The application uses Python's Decimal type for monetary calculations and rounds fares to whole rupees using half-up rounding.

## 9. Smart Card Management

The application supports:

- Standard smart cards.
- Student smart cards.
- Senior citizen smart cards.
- Tourist passes.

Card services include balance top-up, automatic reload, card blocking, tourist pass purchase, and card refund operations.

## 10. Generated Reports

The application generates three CSV reports in the `output` directory.

| Report | Description |
|---|---|
| journey_history.csv | Journey details, entry and exit stations, fares, penalties, and status |
| card_balances.csv | Smart card types, balances, and validity |
| revenue.csv | Fare revenue, penalty revenue, and other revenue |

## 11. Running Tests

The project uses pytest for automated testing.

Run the complete test suite:

```powershell
python -m pytest -q
```

### Latest Verified Test Result

```text
46 passed
```

All 46 automated tests passed in the latest verification.

## 12. Sample Application Execution

The application was successfully executed with the sample CSV input files.

Verified results:

- Stations loaded: 5
- Smart cards loaded: 4
- Events processed: 4
- C001 journey fare: ₹27
- C002 journey fare: ₹12
- Rejected events: 0
- Journey report generated successfully.
- Balance report generated successfully.
- Revenue report generated successfully.

## 13. Documentation

The project includes the following documentation:

- `README.md` – Project overview, features, and setup instructions.
- `design_document.pdf` – Project design documentation.
- `decision_log.md` – Main technical implementation decisions.

## 14. Author Information

**Project ID:** T117-PS-043

**Project Name:** Metro Fare and Smart Card Engine with Zone Fares, Peak Pricing and Penalties

**Programming Language:** Python

**Development Environment:** Visual Studio Code

---

*This README describes the current project implementation and verified test results. Refer to the official problem statement for the complete submission requirements.*

##Demovideo 
[click here to watch the demo](https://drive.google.com/file/d/1O-Sr4HpsVjK6kgPWbhqMeAOaAuQBHfOl/view?usp=drivesdk)