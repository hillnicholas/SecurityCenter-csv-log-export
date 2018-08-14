# SecurityCenter-csv-log-export

A simple CLI tool written in Python 2 to export logs from SecurityCenter 5 in CSV format. This allows for logs to be queried much easier than in the Web UI. 

### Installing 
Python will need to be installed to run this tool. 
The only Python dependency is pySecurityCenter, which can be installed via Pip with the following command:
`pip install pysecuritycenter`

### Usage
There are a number of command line switches that allow for automated scripting. Here are the following command line switches available to use:
`
  -h, --help            show this help message and exit
  -i, --interactive     Use the interactive menu
  -n number_of_logs, --number-of-logs number_of_logs
                        define the number of logs to retrieve (default: 500)
  -o output_filename, --output output_filename
                        define the output file name (default: logs-[current
                        date].csv
  -d date, --date date  define date in format MM/YYYY, i.e. 06/2018
  -H hostname, --host hostname
                        define the hostname of the SecurityCenter instance
`
The date defaults to the current month. If any other parameters are not specified, you will be prompted to enter them interactively. 
