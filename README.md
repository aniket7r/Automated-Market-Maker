# Automated Market-Maker
This is a C++ application that models the behavior of an Automated Market Maker (AMM). To begin using it, just run `make` to compile the code. After that, you can explore various options by passing `-h` or `-help` to understand how to interact with the program.

### Key Features and Options:

- **Help Menu**: Use `-h` or `-help` to display a menu with all available options.
- **Verbose Output**: The `-v` or `-verbose` flag can toggle the detailed transaction logs on or off.
- **Price Statistics**: Want to skip the median price for equities? Add `-m` or `-median` to suppress it.
- **Midpoint Prices**: If you prefer not to print out midpoint prices for equities, use the `-p` or `-midpoint` option.
- **Transfer Details**: You can hide specific transaction details for clients by using `-t` or `-transfers`.
- **Volume Weighted Prices**: Use the `-w` or `-VWAP` command to avoid printing VWAP information.
- **File Input**: Specify an input file with `-f` or `-filename`; otherwise, `test.txt` will be used by default.
- **Custom Delimiters**: You can set your own delimiters with `-d` or `-delimiter`—the default is space and tab.
- **Random Order Flow**: Use `-r` or `-randomOrder` to generate random order flow through a Poisson process, instead of relying on the test file.

### What It Does:
The program processes a mix of buying and selling orders for various stocks or assets. You can either provide predefined streams of data or let the program randomly generate orders using a Poisson distribution. These orders are categorized into different types (like IOC or GTC) and executed by matching buyers and sellers efficiently. Throughout, the system also tracks and computes vital metrics, including the median price, transaction volume, and VWAP (Volume Weighted Average Price) for both equities and participants, while collecting fees from the transactions.
