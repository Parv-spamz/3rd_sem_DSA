# 3rd_sem_DSA
#PARV ARORA - 2401420008

Program Overview
This program is designed to manage temperature records for
multiple years and cities using a two-dimensional list (matrix). It
provides a menu-based interface that lets the user insert, remove,
fetch, and display data in different formats. It also deals with
missing entries and shows the computational complexity of the
operations.
What the Program Does
1. Creates a matrix of size years × cities.
2. Stores and updates temperature values in this matrix.
3. Manages empty/missing entries (sparse data).
4. Prints the data row-wise as well as column-wise.
5. Explains the time and space complexity of operations.
Functions Used
1. __init__(self, years, cities)
Initializes the matrix with None in each cell.
2. populate_auto(self)
Randomly assigns temperatures between 15°C and 40°C
to all cells.
3. insert(self, year, city, temp)
Places a temperature value at the given row (year) and
column (city).
4. delete(self, year, city)
Clears an entry by setting it back to None.
5. retrieve(self, year, city)
Fetches the stored temperature at the given indices.
o Returns "No Data" if missing.
o Returns "Invalid index" if out of range.
6. show_row_major(self)
Displays all values row by row. Missing entries are printed
as "NA".
7. show_column_major(self)
Displays values column by column. Missing entries appear
as "NA".
8. handle_sparse_data(self)
Prints the dataset with "NA" placeholders for missing
information.
9. analyze_complexity(self)
o Insert → O(1)
o Delete → O(1)
o Retrieve → O(1)
o Space → O(years × cities)
