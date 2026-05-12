Interactive Bill Manager<br> 

A robust, command-line interface (CLI) application built in Rust to manage household bills and expenses. This project demonstrates core Rust fundamentals including ownership, mutable borrowing, and efficient data mapping using HashMap.<br>

Features<br>
The application is built in three stages to ensure stability and clean logic:<br>

Stage 1: Management<br>
-Add bills with a unique name and the amount owed.<br>
-View a formatted list of all current bills.<br>

Stage 2: Maintenance<br>
-Remove bills by name from the database.<br>

Stage 3: Refinement<br>
-Edit existing bill amounts.
-"Go Back" Logic: Cancel any action by hitting Enter on an empty prompt to return to the main menu.<br>

Technical Implementation<br>
This project leverages several high-level Rust concepts:<br>
-Data Modeling: Uses struct to define bill attributes and a wrapper struct for the collection logic.<br>
-Collections: Utilizes std::collections::HashMap for $O(1)$ lookups and easy management of unique bill records.<br>
-Input Handling: Features a robust input buffer system that handles user errors and string trimming.<br>
-Memory Safety: Strict adherence to Rust's borrowing rules to ensure data is modified safely across different menu functions.<br>

Installation & Setup<br>
Prerequisites<br>
-Rust Toolchain: Install Rust<br>
Windows Users: Ensure "Desktop development with C++" is installed via the Visual Studio Build Tools.<br>

Steps<br>
-Clone this repository or navigate to your project folder:<br>
Bash<br>
cd bill_manager<br>

Build the project:<br>
Bash<br>
cargo build<br>
Run the interactive menu:<br>
Bash<br>
cargo run<br>

🖥️ Usage Example<br>
Plaintext<br>
--- Bill Manager ---<br>
1. Add Bill<br>
2. View Bills<br>
3. Remove Bill<br>
4. Edit Bill<br>
Enter selection: 1<br>

Bill Name:<br>
> Electricity<br>
Amount:<br>
> 85.50<br>

Bill added.
📝 LicenseThis project was developed as part of the Stellar-Give Bootcamp. Feel free to use, modify, and distribute it for educational purposes.
