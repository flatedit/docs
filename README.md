
![logo.flatedit.com](https://logo.flatedit.com/1/cover.png)

# [docs.flatedit.com](https://bash.flatedit.com/) [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/flatedit/docs/edit/main/DOCS/MENU.md) 

+ [Strona informacyjna: www.flatedit.com](https://www.flatedit.com/)
+ [Dokumentacja - docs.flatedit.com](https://docs.flatedit.com/)
+ [Logotyp: logo.flatedit.com](https://logo.flatedit.com/)
+ [Przykłady - examples.flatedit.com](http://examples.flatedit.com)

+ [LICENSE](../LICENSE)



We started with such script
```bash
#!/bin/bash
## EXAMPLE:
# sh readme.sh
## CONFIG:
FILE_LIST=".readme.txt"
FILE_OUTPUT="README.md"
CONTENT_LIST=$(cat $FILE_LIST)
# START:
echo "<!-- START: This file is rendered, dont' edit it, just separated parts --> " > $FILE_OUTPUT
for content_file in $CONTENT_LIST
do
echo $content_file
if [ -f $content_file ]
then
echo "<!-- $content_file --> " >> $FILE_OUTPUT
cat $content_file >> $FILE_OUTPUT
fi
done
echo "<!-- END: This file is rendered, dont' edit it, just separated parts --> " >> $FILE_OUTPUT
# END
## TEST readme.md
cat README.md
firefox README.md
```


## Contribution [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/flatedit/bash/edit/main/DOCS/START.md)

### Fast Install

```bash
curl https://raw.githubusercontent.com/flatedit/bash/main/flatedit.sh -o flatedit
./flatedit init
```

### Install dependencies after created project

```bash
curl https://raw.githubusercontent.com/flatedit/bash/main/flatedit.sh -o flatedit
echo "https://github.com/flatedit/bash.git flatedit" > "flatedit.dev.txt"
./flatedit install flatedit.dev.txt
```

### install

[minsungson/GitHub-cURL: A guide to installing files from GitHub repos in terminal using cURL](https://github.com/minsungson/GitHub-cURL)

```bash
./flatedit install
```
OR

```bash
./flatedit
```

### init

```bash
./flatedit init
```

### update

```bash
./flatedit update
```


### remove

```bash
./flatedit remove
```


## Contribution [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/flatedit/examples/edit/main/DOCS/CONTRIBUTION.md)


Solutions for development:

### Install

Install dependencies after created project
```bash
curl https://raw.githubusercontent.com/flatedit/bash/main/flatedit.sh -o flatedit
echo "https://github.com/flatedit/bash.git flatedit" > "flatedit.dev.txt"
./flatedit install flatedit.dev.txt
```


Install package list after created project
```bash
curl https://raw.githubusercontent.com/apipackage/bash/main/apipackage.sh -o apipackage
echo "https://github.com/letwhois/bash apidsl/apidsl/bash letwhois" >> "apipackage.txt"
./apipackage install
```

Edit documentation with flatedit
```bash
echo "#!/bin/bash" > "readme"
echo "./flatedit/readme.sh readme.txt" > "readme"
echo "./DOCS/MENU.md" >> "readme.txt"
echo "./DOCS/ABOUT.md" >> "readme.txt"
echo "./DOCS/FOOT.md" >> "readme.txt"
```

### Update documentation

```bash
 ./flatedit
```

### Config project file

The config file: **.flatedit** can be another, e.g. **flatedit.txt**

Just change the first line in  **.flatedit** on **flatedit.txt**
```bash
flatedit.txt
```




## TODO list of flatedit [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/flatedit/docs/edit/main/DOCS/TODO.md)

+ cleaning docs



### ASCIIFlow

[website ASCIIFlow](https://asciiflow.com/#/)
[github lewish/asciiflow: ASCIIFlow](https://github.com/lewish/asciiflow)



### Textik

[website Textik - ASCII diagrams editor](https://textik.com/)
[github flatedit/tixi: Ascii charts editor](https://github.com/flatedit/tixi)



# Tags

+ scripts
+ language


---

+ [edit](https://github.com/flatedit/docs/edit/main/README.md)
+ [flatedit/bash](https://github.com/flatedit/docs)
