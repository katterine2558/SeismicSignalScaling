Signal Processing and DEEPSOIL Results Compiler

This project is a Graphical User Interface (GUI) tool developed using CustomTkinter and Selenium for automating signal processing and compiling DEEPSOIL results. The tool ensures that only authorized devices can execute the application by verifying MAC addresses.

📂 Project Structure

    main.py
    The main script that launches the GUI, verifies MAC addresses, processes seismic signals, and compiles DEEPSOIL outputs.

    prueba.py
    Script for verifying authorized MAC addresses and displaying a basic GUI for authorized users.

    Icons and Images:
        logo.ico: Application icon.
        error.ico: Error icon.
        exito.ico: Success icon.
        progreso.ico: Progress icon.
        icono_escalar.png: Icon for scaling signals.
        icono_postprocesar.png: Icon for compiling DEEPSOIL results.

    requirements.txt
    Dependencies required for the project.

🚀 Features

    MAC Address Verification:
    Ensures that only authorized devices can run the application.

    Signal Processing:
        Select seismic signals from a folder.
        Scale signals by a user-defined factor.
        Generate input files for DEEPSOIL.

    DEEPSOIL Result Compilation:
        Compile results from DEEPSOIL output files.
        Generate consolidated Excel reports with plotted graphs.

    User-Friendly GUI:
        Browse folders and select files via a graphical interface.
        Error and success messages with custom icons.
        Progress windows for tracking task completion.

📋 Prerequisites

    Python 3.x

    Dependencies: Install required libraries with:

    pip install -r requirements.txt

    Dependencies List (from requirements.txt):
        customtkinter == 5.2.1
        gspread == 5.11.2
        numpy == 1.26.4
        openpyxl == 3.1.2
        packaging == 23.2
        pandas == 2.1.1
        pillow == 10.0.1
        uuid == 1.30
        xlsxWriter == 3.1.9
        getmac == 0.9.5

    Google Chrome and ChromeDriver (handled automatically by webdriver_manager).

⚙️ How to Use

    Verify Device Authorization:
        Update the MAC address list in the Google Spreadsheet configured in main.py.

    Run the Application:

    python main.py

    Features:
        Scale Signals:
        Select and scale seismic signals.
        Compile DEEPSOIL Results:
        Compile DEEPSOIL outputs and generate consolidated reports.

🖥️ GUI Screenshots

    Main Menu
    Main Menu

    Signal Scaling
    Signal Scaling

🔒 Security Note

    MAC Address Protection: Only authorized devices can run the application.
    API Keys: Keep service_account.json secure to protect access to the Google Spreadsheet.

🤝 Contributing

Contributions are welcome! Open an issue or submit a pull request to suggest changes.
📝
License

This project is licensed under the MIT License.
