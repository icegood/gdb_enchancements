# gdb_enchancements
To gather all gdb enchancements in one place

## usage
add in .gdbinit (provided you've already had python support)

python
import os
saved_directory = os.getcwd()
end

cd /full/path/to/add_all
source add_all

python
import os
import gdb
os.chdir(saved_directory)
gdb.execute(f'cd {saved_directory}')
end

<other your stuff>
