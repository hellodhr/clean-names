### Clean Names

Takes a csv file with column 'Name' (containing 'dirty names.' For instance, some names may have lastname firstname, others firstname lastname, yet others middlename, lastname, firstname) and returns all the columns of the original csv file + 'uniqid', 'FirstName', 'MiddleInitial/Name', 'LastName', 'RomanNumeral', 'Title', 'Suffix'. By default, it takes out duplicate names.

#### License

Scripts are released under the [MIT License][].

#### Usage

Main: process\_names.py  
process\_names.py calls names.py

#### Command Line Options
<pre><code>
Usage: process_names.py [options]

Options:  
 		-h, 		--help show this help message and exit  
 		-o OUTFILE, --out=OUTFILE  
                  		Output file in CSV (default: sample_output.csv)  
    	-c COLUMN,  --column=COLUMN  
                  		Column name in CSV that contains Names (default: Name)    
    	-a, 		--all      	
    					Export all names (do not take duplicate names out)  (default: False)  
</code></pre>

#### Example
<pre><code>
	python process_names.py -a sample_input.csv  	
</code></pre>

#### Note

The script was used to fix names in CF-Scores from [Database on Ideology, Money in Politics, and Elections][]. Processed database with clean names posted on [Harvard DVN][].

  [MIT License]: https://github.com/soodoku/Clean-Names/blob/master/License.md
  [Database on Ideology, Money in Politics, and Elections]: http://data.stanford.edu/dime 
  [Harvard DVN]: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/28949
 

