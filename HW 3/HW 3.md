### bash script
tree.sh
```vim 
#!/bin/bash
FIL_DIR=`ls`
for val in $FIL_DIR
do
        if [ -f $val ]; then
                echo "$val" >> filename.txt
        elif [ -d $val ]; then
                echo "$val" >> dirname.txt
        fi
done
exit 0
```
### running result
1. filename.txt
```
root@bioinfo_docker:/home/test/share/bash_homework/bash_homework# cat filename.txt 
a1.txt
a.txt
b1.txt
bam_wig.sh
b.filter_random.pl
c1.txt
chrom.size
c.txt
d1.txt
dir.txt
e1.txt
f1.txt
human_geneExp.txt
if.sh
image
insitiue.txt
mouse_geneExp.txt
name.txt
number.sh
out.bw
random.sh
read.sh
test3.sh
test4.sh
test.sh
test.txt
tree.sh
wigToBigWig
```
2. dirname.txt
```
root@bioinfo_docker:/home/test/share/bash_homework/bash_homework# cat dirname.txt 
a-docker
app
backup
bin
biosoft
c1-RBPanno
datatable
db
download
e-annotation
exRNA
genome
git
highcharts
home
hub29
ibme
l-lwl
map2
mljs
module
mogproject
node_modules
perl5
postar2
postar_app
postar.docker
RBP_map
rout
script
script_backup
software
tcga
test
tmp
tmp_script
var
x-rbp
```