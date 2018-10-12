# desarrolla2/file fork

This provide a simple api to read and write files.

This repository is for maintaining desarrolla2/file used in legacy software, and should not be used or published to packagist.

## Installation with Composer
Add the repository to the project composer.json:

``` json
    "repositories": [
        { "type": "vcs", "url": "https://github.com/raid-software/File" },
    ],
```

continue by adding `desarrolla2/file` to the required packages section.

``` json
    "require": {
        "desarrolla2/file":  "*"
    }
```

### Without Composer

You can also download it from [Github] (https://github.com/desarrolla2/File),  but no autoloader is provided so 
you'll need to register it with your own PSR-4  compatible autoloader.

## Usage
   
``` php   
<?php
require __DIR__ . '/../vendor/autoload.php';

use Desarrolla2\File\File;

// Simple api to write file

File::write($fileName,$data);

// Simple api to read file

File::read($fileName);

```

## Formats

Current supported formats are:

- File: raw data
- Json: encode arrays to json files.

## Contact

You can contact with me on [@desarrolla2](https://twitter.com/desarrolla2).
