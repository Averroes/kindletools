The KindleTools Project

Author: Plamen Valov
License: GPL
Version: 0.1
Date: 25.02.2012
Contact: paco09@abv.bg
Copyright 2012, The Kindle Tools Project


Tools Description:

    * collgen.py
    ----------------------------------------------------------------------------
    Usage: collgen.py [options]
    
    Generates collections.json file from a given path. Calculates collections
    based on the directory structure where books reside
    
    Options:
      -h, --help            show this help message and exit
      -d BOOK_DIRECTORY, --book-directory=BOOK_DIRECTORY
                            Book directory which is used to generate
                            collections.json from
      -o OUTPUT_JSON_PATH, --output-json-path=OUTPUT_JSON_PATH
                            Location where collections.json will be generated
    ----------------------------------------------------------------------------
    Example:
    
    $> python collgen.py -d /media/Kindle/documents -o /media/Kindle/system
      Collections file written to:
      /media/Kindle/system/collections.json
    ----------------------------------------------------------------------------
