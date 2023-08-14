# pdf-with-python
A simple repository to show how I've used pypdf2 library to extract information from a .pdf file. The main reason to do this, is that most of the functions and methods described on internet are deprecated, so I've created this repository to update the information (and to save the scripts I develop at my full time job).

Basically, what I needed to do was to retrieve the names of clientes from a .pdf file that had more than 1000 pages - it was impracticable to do it by hand. Each page corresponded to one client, so it was pretty straightfoward to get the information. Luckily, the string "NOME" (name in portuguese) only showed up once, so I just had to iterate over the pages and use the .find function to gather the names. Finally, I've put everything into a pandas DataFrame and exported to Excel (.xlsx file).

I've writed the script into a jupyter notebook.
