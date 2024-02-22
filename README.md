# Algorithm for file updates in Python
# This project was made with files used in the Google Cybersecurity Certificate 
# Assign 'import_file' to the name of the file
import_file = "allow_lists.txt"

# Building a with statement to read the contents of the file
with open (import_file, "r") as file:

  # Use the read command to read the imported file and store it in a variable named 'ip_addresses'
  ip_addresses = file.read()

# Convert the string into a list
ip_addresses = ip_addresses.split()

# Iterate through the remove list
for element in remove_list: 

  # Build conditional statement if current element is in ip_addresses
  if element in ip_addresses:

  # The current element should be removed from ip_addresses
    ip_addresses.remove(element)
    
# Convert ip_addresses back into a string so that it can be written into a text file
ip_addresses = "\n".join(ip_addresses)

# Build a with statement to rewrite the original file
with open(import_file, "w") as file:

  # Rewrite the file, replacing its contents with 'ip_addresses'
  file.write(ip_addresses)

# Here is a document showing what I did more in depth and why
[Algorithm for file updates in Python.pdf](https://github.com/JayceR01/Python-update/files/14378880/Algorithm.for.file.updates.in.Python.pdf)
