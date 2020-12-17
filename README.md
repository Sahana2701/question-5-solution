Question 5 solution
5.a
def unique update (data1,data2):
#initially empty dictionary
dup keys ={}
#examine every (k,V2) pair in data 2
for [k,v2] in data2:
#check if there is a key value
#pair with key=k in data 1 if k in data1:
V1=data1[k] 
#(k,v1)in dict1
#check if v1!=V2
if v1!=V2:
#add(k,[v1,V2])
#to dictionary
dup keys [k]=[v1,v2] from data1
Adel data1[k]
else:
#add (k,v2) to data 1 
data1[k]=V2
#After processing all (k,V2)in #data2, return the dictionary return dup keys

5.b
if k in data1:
V1= data1[k]
if v1!= V2:
dup keys[k]=(v1,V2)
del data1[k]
else:
data1[k]=V2
return dup keys 

5.c
Test case1
1 2
3 3
3 8 
4 9
2
3 3
4 4
Test case 2
4
1 2
2 2
3 3
4 19
2
3 3
4 19

Test case 3:
The test case written in 5a,which breaks the initially written code can be written
