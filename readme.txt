THE DATASET
# SUMMARY
VERSION		Number of Characters	Number of Classes	Data			Contained characters
--------------------------------------------------------------------------------------------------------------------
Version I	156000			78			Original + Augmented	English, Hungarian, Turkish
Version II	24000			12			Original + Augmented	Turkish special
Version III	36000			18			Original + Augmented	Hungarian special
Version IV	104000			52			Original + Augmented	English
Version V	156000			55			Original + Augmented	English, Hungarian, Turkish
Version VI	78000			78			Original		English, Hungarian, Turkish
# VERSIONS
Version I: This version represents the entire dataset. It includes all the 28x28 pixel binary characters from the three alphabets together forming a balanced dataset with 156000 characters belonging to 78 classes.
Version II: It consists of merely 12 Turkish special characters (6 upper-case and 6 lower-case). 2000 samples of each character can be found in the Version II forming a 24000-character dataset.
Version III: Similar to the Version II, this includes 18 Hungarian special characters only (9 lower-case and 9 upper-case) forming a 36000-character dataset.
Version IV: The fourth version includes 2000 samples of 52 English characters (26 upper-case and 26 lower-case). 
This representation enables us to merge English letters with Hungarian special Characters and work only on Hungarian characters by just putting two versions together. A fair warning should be provided about the Turkish alphabet; putting Version II and Version IV together does not result in the Turkish alphabet since there are no letter “q”,” w” and “x” in the Turkish alphabet. The users may want to exclude those 3 letters (3 lower-case and 3-upper-case) from the Version 4 in order to work on Turkish alphabet accurately.
Version V: This version is derived from the Version I type which includes all the characters from different alphabets together. The characters having a similar way of representation in their upper-case and lower-case form are put into the same class in this version such as lower case “o” and upper case “O”. The characters merged are shown in the MERGED CLASSES section below. In this group there are 55 classes and 156000 samples. However, only in this version the number of instances in each class is not balanced. Some classes have 2000 samples whereas merged ones are represented in 4000 samples. 
Version VI: The original handwritten characters (1000 instances for every 78 classes) are put forward in the sixth version. Using this version, it is possible to experiment different distortion techniques and their impact on the classification performance can be tested. 78000 characters from 78 different classes can be found in this version. 

# CLASSES LABELS
a-1	t-20	A-40	U-60
b-2	u-21	B-41	V-61
c-3	v-22	C-42	W-62
d-4	w-23	D-43	X-63
e-5	x-24	E-44	Y-64
f-6	y-25	F-45	Z-65
g-7	z-26	G-46	Ç-66
h-8	ç-27	H-47	Ğ-67
i-9	ğ-28	I-48	İ-68
j-10	ı-29	J-49	Ş-69
k-11	ş-30	K-50	Ö-70
l-12	ö-31	L-51	Ü-71
m-13	ü-32	M-52	Á-72
n-14	á-33	N-53	É-73
o-15	é-34	O-54	Í-74
p-16	í-35	P-55	Ó-75
q-17	ó-36	Q-56	Ő-76
r-18	ő-37	R-57	Ú-77
s-19	ú-38	S-58	Ű-78
	ű-39	T-59	

# MERGED Classes
a	1	l	12	w-W	23	é	34	G	45
b	2	m-M	13	x-X	24	í-Í	35	H	46
c-C	3	n	14	y-Y	25	ó-Ó	36	L	47
d	4	o-O	15	z-Z	26	ő-Ő	37	N	48
e	5	p-P	16	ç	27	ú-Ú	38	Q	49
f	6	q	17	ğ	28	ű-Ű	39	R	50
g	7	r	18	ı-İ	29	A	40	T	51
h	8	s-S	19	ş-Ş	30	B	41	Ç	52
i-I	9	t	20	ö-Ö	31	D	42	Ğ	53
j-J	10	u-U	21	ü-Ü	32	E	43	Á	54
k-K	11	v-V	22	á	33	F	44	É	55


# MERGED Letters
c- C	s-S
i-I	ş-Ş
í- Í	u-U
ı-İ	ú -Ú
j-J	Ü-Ü
k-K	ű- Ű
m-M	v-V
o-O	w-W
ó- Ó	x-X
Ö-Ö	y-Y
ő- Ő	z-Z
p-P	
