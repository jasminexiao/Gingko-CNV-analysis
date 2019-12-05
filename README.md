# Gingko-CNV-analysis
sample list:
Icm01.W.s12---46,XY(CNV pattern)
Icm03.W.s58---46,XX
Icm10.Q.s246---46,XX

bed files:
Icm01.W.s12.bed
Icm03.W.s58.bed
Icm10.Q.s246.bed

Use different rerfence:
1.reference:Icm03.W.s58---46,XX
output:Icm01.W.s12---46,XY
       Icm10.Q.s246---46,XX

2.reference:Icm01.W.s12---46,XY
output:Icm10.Q.s246---46,XX
       Icm03.W.s58---46,XX

My comments:
1.reference:Icm03.W.s58---46,XX
The output are right.
2.reference:Icm01.W.s12---46,XY
The output are wrong,because chrY is one copy, chrX is two copy, all samples are diploids. So chrX should be 4 copy, but the output is 2 copy. I think the parameter segMeth=2 in config file didn't work.

