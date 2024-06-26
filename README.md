# PDF Editor

This Python script provides a graphical user interface (GUI) for performing various operations on text and PDF files. It allows users to convert text files to PDF, split PDFs, merge PDFs, convert PDFs to images, and convert PDFs to PowerPoint presentations.

## Features

- Convert text files to PDF format
- Convert Image files to PDF format
- Split PDF files into multiple PDFs
- Merge multiple PDF files into a single PDF
- Convert PDF files to image format (PNG, JPG, etc.)
- Convert PDF files to PowerPoint presentations

## Dependencies

Ensure you have the following dependencies installed:

- **tkinter**: Python's standard GUI (graphical user interface) toolkit.
- **os**: Provides a portable way of using operating system-dependent functionality.
- **shutil**: Provides a higher-level interface for file operations.
- **filedialog** from tkinter: Provides dialogs for opening and saving files.
- **pathlib**: Provides classes representing filesystem paths.
- **fpdf**: A Python library for generating PDF files.
- **PyPDF2**: A Python library to work with PDF files.
- **pdf2image**: A Python library to convert PDFs to images.
- **dotenv**: A Python library to manage environment variables.
- **groupdocs_conversion_cloud**: A Python library for converting documents, powered by GroupDocs.
- **img2pdf**: A Python library for converting images into PDF files.

## Setup

1. Clone this repository to your local machine.

```bash
git clone https://github.com/Sahil-Chhoker/PDF-Editor.git
```

2. Navigate to the project directory.

```bash
cd PDF-Editor
```

3. Create a virtual environment (optional but recommended).

```bash
python -m venv env
source env/bin/activate  # On Windows, use `env\Scripts\activate.ps1`
```

4. Install the required dependencies using pip.

```bash
pip install -r requirements.txt
```

### Installing Poppler
**NOTE**: You ONLY need popler if you are converting your pdf to images, the rest works okay.

1.
   **For Windows Users:**
   - Go to the [Poppler Windows Releases](https://github.com/oschwartz10612/poppler-windows/releases) page.
   - Download and install the latest release of Poppler for Windows.
   - Once installed, locate the path to the `bin` directory of your Poppler installation.
     
   **For Mac and Linux Users:**
   - Visit the [Poppler Official Website](https://poppler.freedesktop.org/).
   - Download and install the latest release of Poppler for your OS.
   - Once installed, note down the path to the `bin` directory of your Poppler installation.

3. **Specify Poppler Path in the Script:**
   - Open the `.env` file in your PDF Editor project directory.
   - Replace the placeholder `your_poppler_path` with the actual path to the `bin` directory of your Poppler installation.


6. Set up environment variables for authentication with the GroupDocs API. Create a `.env` file in the root directory of the project and add your client ID and client secret. (For more information on getting your credentials, visit [GroupDocs Dashboard](https://dashboard.groupdocs.cloud/))

   **NOTE**: You only need the API credentials ONLY if you are converting pdf to pptx, everything else works on your local machine.

```
CLIENT_ID=your_client_id_here
CLIENT_SECRET=your_client_secret_here
POPPLER_PATH=your_poppler_path
```

## Usage

1. Run `python main.py` in your terminal.
2. Click on an operation button to start.
3. Follow on-screen prompts to select files and folders.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Author

Sahil Chhoker
