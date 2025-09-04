# Hazardous Waste Information Platform (HWIP)

This repository houses the public help center content for RCRAInfo's Hazardous Waste Information Platform. 

## Local Development

### Prerequisites

- Python
    - I recommend [uv](https://docs.astral.sh/uv/) for especially for EPA employees since it makes installing 
      Python and setting up virtual environments easier without going through EISD much easier.
    - See [the uv installation guide](https://docs.astral.sh/uv/getting-started/installation/) for more information.

### Setup

Assuming you are using a unix-like terminal or Windows PowerShell.

1. Clone the repository:

    ```shell
    git clone https://github.com/USEPA/hwip.git
    cd hwip
    ```

2. Create and activate a virtual environment:

    ```shell
    uv venv  # will create a .venv directory
    # if not using uv, you can create a venv with `python -m venv .venv`
    . .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
    ```

3. Install dependencies:

    ```shell
    uv sync
    # if not using uv, python -m pip install .
    ```

4. Start the development server:

    ```shell
    mkdocs serve
    # Should output a local URL like http://127.0.0.1:8000 to view the site in your browser.
    ```
