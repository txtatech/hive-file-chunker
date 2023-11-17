# hive-file-chunker
A method to gzip, base64 encode and chunk local files into JSON format to fit in a single block on the Hive blockchain.

To encode local files into JSON format place them in the inputs folder.

The 'Build_GPT_Buddy.zip' is included in the 'inputs' folder as an example.

The current chunk size (for the character count inside the JSON files) is set to 64536.

A single block (on the Hive Blockchain) can contain 65536 charaters so I left some margain for error.

# Encoding Step:

Note that all files to be encoded should be placed in the 'inputs' directory.
Note that the JSON files are output to the 'outputs/chunks' directory.

To encode files do:

~~~
python3 hive_file_chunker.py
~~~

# Decoding Step:

Note that the  files are output to the 'outputs/chunks' directory.

To decode files do:

~~~
python3 hive_file_dechunker.py
~~~
