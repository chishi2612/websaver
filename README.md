# websaver
Extensible web content downloader

### Installation

From npm

[![NPM](https://nodei.co/npm/websaver.png)](https://npmjs.org/package/websaver)
```
npm install -g websaver
```

From source
```
git clone https://github.com/jul11co/websaver.git
npm install -g websaver/
```

### Usage
Currently, supports downloading images from some manga sites.

```
Download page to local directory
    websaver download <page_url> <output_dir> [--force]
    
Update local directory
    websaver update <output_dir>
    
Add page to download list (into state file in parent directory)
    websaver add-page <page_url> <output_dir>
    
Download images to local directory
    websaver download-image <page_url> <output_dir> [SELECTOR]
    
Run script
    websaver run-script <SCRIPT-FILE> <page_url> <output_dir>
```

### Customize

Write [EJS](https://github.com/mde/ejs) script and run it with
```
websaver run-script <SCRIPT-FILE> <page_url> <output_dir>
```
See examples in scripts/

### License

Licensed under the Apache License, Version 2.0
(<http://www.apache.org/licenses/LICENSE-2.0>)
