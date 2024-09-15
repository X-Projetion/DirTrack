# DirTrack

**Description:** DirTrack is a directory scanning tool designed to explore and discover files and directories on websites with an "index of" view. With the ability to scan directory structures, this tool provides useful information about the files present in directories and their display.

## Key Features

- **Directory Scanning:** Traverses directories and subdirectories to find files and folders listed in an "index of" view.
- **File Detection:** Identifies files with specific extensions such as `.php`, `.sh`, and others that might contain sensitive information.
- **Content Checking:** Examines file content for specific elements such as the keyword "password" and provides a report of the findings.
- **Detailed Output:** Provides a comprehensive report including file status, size, and the first line of file content if required.
- **Multi-Threading:** Supports scanning with multiple threads to improve speed and efficiency.

## How It Works

DirTrack scans directories from a specified URL and processes the list of files and directories found. The tool gathers information about file sizes, HTTP status codes, and file content (first line) to provide an overview of the available content on the website.

## Benefits

DirTrack is useful for developers, system administrators, and security professionals who need to explore and audit directory structures and files on websites. With efficient scanning and tracking capabilities, this tool helps in identifying potential security issues and ensuring content integrity.

## Requirements

- Python 3.x
- `requests` and `BeautifulSoup` libraries

## Installation

1. **Clone this repository:**

    ```bash
    git clone https://github.com/X-Projetion/DirTrack.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd DirTrack
    ```

3. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Run DirTrack:**

    ```bash
    python DirTrack.py -u [TARGET_URL] -t [NUMBER_OF_THREADS]
    ```

    - `-u` or `--url`: Target URL to scan.
    - `-t` or `--threads`: Number of threads to use for scanning.

## Usage Example

```bash
python dirtrack.py -u http://example.com -t 5
