# docs-template

Template for websites and documentation pages in the style of [developerc76.github.io](https://developerc76.github.io/)

## Requirements: 

Racket (> 8.1), Raco, Bash, wget, unzip

## Directions: 

### Clone the template

#### Option 1: 

Download the zip file for the template and unzip the folder: 

```
$ wget https://raw.githubusercontent.com/developerc76/docs-template/main/docs.zip
$ unzip docs.zip
```

#### Option 2: 

Run the following in the repo in which the template should be placed: 

This will clone the template to a new folder in the repo called docs/

```
$ git clone https://github.com/developerc76/docs-template.git
$ cd docs-template
$ mv docs ..
$ cd .. && rm -rf docs-template
```

### Install dependencies

Install Pollen (Update if needed): 

```
$ sudo raco pkg install pollen
```

### How to run

Write markdown into the info.html.pmd file (KEEP THE "#lang pollen" in the first line)

```
$ chmod +x compile.sh
$ ./compile.sh
```

Run locally at [port 8080](http://localhost:8080/index.ptree) by default (by clicking on the index.html file)

Deploy on GitHub Pages or GitLab Pages (they will use the index.html file as the file to render at username.github.io/project/)

## Notes: 

Tested on Racket 8.7 (Debian 12)

Used Pollen v3.2

This is mobile and desktop friendly

Example of this template: [GitHub pages for this repo](https://developerc76.github.io/docs-template/)

After headings like "# Heading" or "## Heading 2", you should add a "\<br>" statement