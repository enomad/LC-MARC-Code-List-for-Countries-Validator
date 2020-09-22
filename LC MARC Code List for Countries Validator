#Program compares LC country codes, saved as codes.txt, to a list of codes extracted from MARC records (MARC 008_15-17 - Place of publication, production, or execution). The program prints any codes that are not valid to the screen.


#read all codes from the textfile into a list
with open('ccodes.txt', 'r') as f:
    
    content = f.readlines()

    content = [x.strip() for x in content] 

#Read a file containing MARC 008_15-17 codes e into a list

with open('marc.txt', 'r') as g:

    marc_content = g.readlines()

    marc_content = [x.strip() for x in marc_content] 

#Method 1:

set_difference = set(marc_content) - set(content)

list_difference = list(set_difference)

print(list_difference)

#Method 2:
s = set(content)


results = [x for x in marc_content if x not in s]

print(results)

