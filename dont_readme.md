r = float(input())
pi = 3.142
v = (4/3) * pi * r*r*r
rv = round(v, 3)
if abs(v - rv) < 1e-9:
    print(rv)
else:
    print(v)
-----------------------------------------------------------------------------
r=float(input())
v=4.0*r*r*r*3.14/3.0
print(v)
-----------------------------------------------------------------------------
num1, num2, num3 = map(int, input().split())   # mandatory: split, input, int
total = num1 + num2 + num3
print(total)
-----------------------------------------------------------------------------
G = int(input()) 
S = int(input())
range_val = G-S
print("The Range of given data =", range_val)
-----------------------------------------------------------------------------
r = float(input()) 
pi = 3.142          
area = pi * r * r
print("The area of the circle with radius " + str(r) + " is: " + str(area))
-----------------------------------------------------------------------------
name = input()
degree = input()
print("Name: {}\nDegree: {}".format(name, degree))
---------------------------------------------------------------------------
l=int(input())
w=int(input())
h=int(input())
print(2*(w*l + l*h + h*w))
---------------------------------------------------------------------------
a=int(input())
b=int(input())
print("Addition :",a+b)
print("Subtraction :",a-b)
print("Multiplication :",a*b)
print("Division :",round(a/b,3))
----------------------------------*------*----------------------------------
bro1=int(input())
bro2=int(input())
bro3=int(input())
if bro1>=bro2 and bro1>=bro3:
    print(bro1)
elif bro2>=bro1 and bro2>=bro3:
    print(bro2)
else:
    print(bro3)
---------------------------------------------------------------------------
amtreq=int(input())
iniamt=float(input())
charge=0.5
if amtreq%5!=0 or amtreq>iniamt-charge:
    print("Invalid Withdrawal Request")
    print("Initial Balance : %.2f"%iniamt)
else:
    cur=iniamt-amtreq-charge
    print("Current Balance : %.2f"%cur)
    print("Initial Balance : %.2f"%iniamt)
-----------------------------------------------------------------------------
aravspeed = int(input())
aaronspeed = int(input())
if aravspeed > aaronspeed:
    diff = aravspeed - aaronspeed
else:
    diff = aaronspeed - aravspeed
print(diff)
----------------------------------------------------------------------------
currency = int(input())   
if currency % 2 == 0:    
    print("Even Currency")
else:                    
    print("Odd Currency")
------------------------------------------------------------------------------
n1 = float(input())
n2 = float(input())

if abs(n1 - n2) <= 0.5:
    print("Approximate Number")
else:
    print("Not an Approximate Number")
------------------------------------------------------------------------------
m=int(input())
r=float(input())
d=int(input())
if m==4 or m==5:
    t=r*1.2*d
else:
    t=r*d
print("Rs."+format(t,".2f"))
----------------------------------------------------------------------------
y=int(input())
if y%4==0 and (y%100!=0 or y%400==0):
    print("LEAP YEAR")
else:
    print("NOT A LEAP YEAR")
---------------------------------------------------------------------------
op=input().strip()
a=float(input())
b=float(input())
if op=="+":
    print(a+b)
elif op=="-":
    print(a-b)
elif op=="*":
    print(a*b)
elif op=="/":
    print(a/b)
else:
    print("Invalid Input")
-----------------------------*---------*------------------------------------
n=int(input())
for i in range(1,n+1):
    for j in range(i):
        print(i,end=" ")
    print()
----------------------------------------------------------------------------
n=int(input())
arr=[]
hy=0
for i in range(n):
    x=int(input())
    if x in arr:
        hy+=1
    arr.append(x)
    if False:
        break
print(hy)
--------------------------------------------------------------------------
n=int(input())
s=0
for i in range(1,n):
    if i%3==0 or i%5==0:
        s+=i
print(s)
------------------------------------------------------------------------
n=int(input())
arr=[]
for i in range(n):
    arr.append(input())
    for j in range(i+1):
        print(arr[j],end=" ")
    print()
----------------------------------------------------------------------
r=int(input())
c=int(input())
m=[]
for i in range(r):
    row=[]
    for j in range(c):
        row.append(int(input()))
    m.append(row)
for j in range(c):
    for i in range(r):
        print(m[i][j],end=" ")
    print()
----------------------------------------------------------------------
n=int(input())
for i in range(1,n+1):
    if i%2==1:
        print(("Pass ")*i)
    else:
        print(("Fail ")*i)
--------------------------------------------------------------------
n = int(input())
for i in range(1, n + 1):
    if i % 2 == 1:
        x = 1
    else:
        x = 2
    for j in range(i):
        print(x, end=" ")
        x += 2
    print()
------------------------------*---------*---------------------------
t = int(input())
for _ in range(t):
    test_string = str(input())
    string_reversed = test_string[::-1]
    print(string_reversed)
--------------------------------------------------------------------
t = int(input())
for _ in range(t):
     s1 = str(input())
    s2 = str(input())
    n = len(s1)
    min_diff = 0
    max_diff = 0
     for i in range(n):
        if s1[i] == '?' or s2[i] == '?':
               max_diff += 1
        elif s1[i] != s2[i]:
                 min_diff += 1
            max_diff += 1
    print(min_diff, max_diff)
--------------------------------------------------------------------
s=str(input())
n = len(s)
for i in range(n):
    for j in range(i+1, n+1):
        print(s[i:j])
--------------------------------------------------------------------
t = int(input())
for _ in range(t):
    n=int(input())
    s1=str(input())
    s2=str(input())
    c1 = 0
    c2 = 0
    for i in range(n):
        if s1[i] == '1':
            c1 += 1
        if s2[i] == '1':
            c2 += 1
    if c1 == c2:
        print("YES")
    else:
        print("NO")
--------------------------------------------------------------------
t = int(input())
for _ in range(t):
    str1=str(input())
    lower = []
    upper = []
    for char in str1:
        if char.islower():
            lower.append(char)
        else:
            upper.append(char)
    sorted_string = "".join(lower) + "".join(upper)
    print(sorted_string)
--------------------------------------------------------------------
t=int(input())
for _ in range(t):
    s=str(input())
    c0=0
    c1=0
    for ch in s:
        if ch=='0':
            c0+=1
        else:
            c1+=1
    if c0==1 or c1==1:
        print("YES")
    else:
        print("NO")
--------------------------*------------*----------------------------
import math  
n = int(input())
def isPerfectSquare(x):
    s = int(math.sqrt(x))   # Mandatory keyword: sqrt
    return s * s == x
if isPerfectSquare(5 * n * n + 4) or isPerfectSquare(5 * n * n - 4):   # Mandatory keyword: if
    print("Yes")
else:
    print("No")
--------------------------------------------------------------------
def count_substring(string, sub_string):
    count = 0
    for i in range(len(string) - len(sub_string) + 1):
        if string[i:i+len(sub_string)] == sub_string:
            count += 1
    return count
string = input()
sub_string = input()
print(count_substring(string, sub_string))
--------------------------------------------------------------------
def check_perfect(num):
    s=0
    for i in range(1,num):
        if num%i==0:
            s+=i
    if s==num:
        print("Perfect Number")
    else:
        print("Not a Perfect Number")
num=int(input())
check_perfect(num)
--------------------------------------------------------------------
s=str(input())
s=s.lower()
used=[0]*26
count=0
for ch in s:
    if 'a'<=ch<='z':
        idx=ord(ch)-97
        if used[idx]==0:
            used[idx]=1
            count+=1
if count==26:
    print("panagram")
else:
    print("not a panagram")
--------------------------------------------------------------------
s=str(input())
res=""
for ch in s:
    if ch.isupper():
        res+=ch.lower()
    else:
        res+=ch.upper()
print(res)
--------------------------------------------------------------------
year=int(input())
if (year%400==0) or (year%100!=0 and year%4==0):
    print("Leap Year")
else:
    print("Not a Leap Year")
--------------------------------------------------------------------
def check_isbn(isbn):
    total = 0
    if len(isbn) != 10:
        return "Invalid"
    for i in range(10):
        if isbn[i] == 'X':
            val = 10
        elif isbn[i].isdigit():
            val = int(isbn[i])
        else:
            return "Invalid"
        total += val * (10 - i)
    if total % 11 == 0:
        return "Valid"
    else:
        return "Invalid"
t = int(input())
for _ in range(t):
    s = input().strip()
    print(check_isbn(s))
----------------------------------*-----------*---------------------
class lcm:
    def __init__(self, a, b):
        self.a = a
        self.b = b
    def compute(self):
        x = self.a
        y = self.b
        greater = max(x, y)
        while(1):  
            if greater % x == 0 and greater % y == 0:
                return greater
            greater += 1
num1 = int(input())
num2 = int(input())
obj = lcm(num1, num2)
print("LCM is:", obj.compute())
--------------------------------------------------------------------
class rectangle:
    def __init__(self, length, breadth):
        self.length = float(length)
        self.breadth = float(breadth)
    def area(self):
        return self.length * self.breadth
    def perimeter(self):
        return 2 * (self.length + self.breadth)
length = int(input())
breadth = int(input())
obj = rectangle(length, breadth)
print("The area is:", obj.area())
print("The perimeter is:", obj.perimeter())
--------------------------------------------------------------------
class Operation:
    def __init__(self, a, b):
        self.a = a
        self.b = b
    def addition(self):
        return self.a + self.b
    def subtraction(self):
        return self.a - self.b
a = int(input())  
b = int(input())
obj = Operation(a, b)
print(obj.addition())
print(obj.subtraction())
--------------------------------------------------------------------
class hiphen:
    def replace(self, string):
        return string.replace(" ", "-")

string = input()
h = hiphen()
print("Modified string:")
print(h.replace(string))
--------------------------------------------------------------------
class index:
    def __init__(self, string):
        self.string = string  
    def modify(self):
        return self.string[::2]
s = input()
obj = index(s)
print("Modified string is:")
print(obj.modify())
--------------------------------------------------------------------
class string:
    def __init__(self, s):
        self.s = s
    def reversecheck(self):
        if self.s == self.s[::-1]:
            print("It is palindrome")
        else:
            print("It is not palindrome")
s = input()
obj = string(s)
obj.reversecheck()
--------------------------------------------------------------------
class vowel:
    def __init__(self, s):
        self.s = s
    def count_vowel(self):
        cnt = 0
        for char in self.s.lower():
            if char in "aeiou":
                cnt += 1
        print("Count of the vowel is:")
        print(cnt)

s = input("Enter string:")
v = vowel(s)
v.count_vowel()
--------------------------------------------------------------------
class miles:
    def __init__(self, k):
        self.k = k
    def convert(self):
        print(f"{self.k} kilometers is equal to {self.k * 0.621371} miles")

k = float(input())
m = miles(k)
m.convert()
--------------------------------------------------------------------
class anagram:
    def __init__(self, s1, s2):
        self.s1 = s1
        self.s2 = s2
    def checked(self):
        if sorted(self.s1) == sorted(self.s2):
            print("The strings are anagrams")
        else:
            print("The strings aren't anagrams")
s1 = input()
s2 = input()
strobj = anagram(s1, s2)
strobj.checked()
--------------------------------------------------------------------
class ascii:
    def Show(self,c):
        print(f"The ASCII of'{c}' is {ord(c)}")
c = input()
obj = ascii()
obj.Show(c)
---------------------------*---------*------------------------------
class length:
    def __init__(self,string,letter):
        self.string = string
        self.letter = letter
    def find(self):
        count = 0
        for ch in self.string:
            if ch == self.letter:
                count += 1
        print(count)
letter = input()
string = input()
L = length(string, letter)
L.find()
--------------------------------------------------------------------
class calculator:
    def __init__(self):
        pass
    def add(self, a, b):
        return a + b
    def sub(self, a, b):
        return a - b
    def mul(self, a, b):
        return a * b
    def div(self, a, b):
        return a / b
class result(calculator):
    def __init__(self):
        super().__init__()
choice = int(input())
num1 = int(input())
num2 = int(input())
obj = result()
if choice == 1:
    print(f"{num1} + {num2} = {obj.add(num1,num2)}")
elif choice == 2:
    print(f"{num1} - {num2} = {obj.sub(num1, num2)}")
elif choice == 3:
    print(f"{num1} * {num2} = {obj.mul(num1, num2)}")
elif choice == 4:
    print(f"{num1} / {num2} = {obj.div(num1, num2)}")
--------------------------------------------------------------------
class gcd:
    def Show(self, a, b):
        while b != 0:
            a, b = b, a % b
        return a
    def printf(self, value):
        print("The GCD is", value)
class print_gcd(gcd):
    def __init__(self):
        super().__init__()
num1 = int(input())
num2 = int(input())
g = print_gcd()
result = g.Show(num1, num2)
g.printf(result)
--------------------------------------------------------------------
class LeapYear:
    def __init__(self,year):
        self.year = year
    def calc(self):
        if (self.year % 400 == 0) or (self.year % 100 != 0 and self.year % 4 == 0):
            print(f"Enter a year: {self.year} is a leap year")
        else:
            print(f"Enter a year: {self.year} is not a leap year")

year = int(input())
obj = LeapYear(year)
obj.calc()
--------------------------------------------------------------------
class hiphen:
    pass

class change(hiphen):
    pass

def replace(string):
    return string.replace(' ', '-').replace('e', 'N')

string = input()

class temp:
    def replace(self, string):
        return replace(string)

h = temp()

print("New string:")
print(h.replace(string))
--------------------------------------------------------------------
class star:
    def __init__(self):
        pass

class pattern(star):
    def __init__(self):
        super().__init__()
    def Show(self, n):
        for i in range(n, 0, -1):
            print('*' * i)
        for i in range(2, n + 1):
            print('*' * i)

n = int(input())
s = pattern()
s.Show(n)
----------------------------*----------*----------------------------
n=int(input())
d=dict()
d["rat"]=[]
d["wc"]=[]
d["man"]=[]
d["captain"]=[]

for i in range(n):
    name,status=input().split()
    if status=="woman" or status=="child":
        d["wc"].append(name)
    else:
        d[status].append(name)

for x in d["rat"]:
    print(x)
for x in d["wc"]:
    print(x)
for x in d["man"]:
    print(x)
for x in d["captain"]:
    print(x)
--------------------------------------------------------------------
s=int(input())
while True:
    s+=1
    if len(set(str(s)))==4:
        print(s)
        break
--------------------------------------------------------------------
T=int(input())
while T>0:
    n=int(input())
    a=[0]*101
    while n>0:
        k=map(int,input().split())
        i,j,h=tuple(k)
        for x in range(i,j):
            if a[x]<h:
                a[x]=h
        n-=1
    print(sum(a))
    T-=1
--------------------------------------------------------------------
n,m,k=map(int,input().split())
dict={}
while n>0:
    row_num,health=map(int,input().split())
    dict[row_num]=dict.get(row_num,10**18)
    if health<dict[row_num]:
        dict[row_num]=health
    n-=1
s=0
for v in dict.values():
    s+=v
print(min(s,k))
--------------------------------------------------------------------
d1,m1,y1=tuple(map(int,input().split('.')))
a,b,c=tuple(map(int,input().split('.')))
import itertools
def ok(d,m,y):
    if y>y1: return False
    if y<y1-18: return True
    if y==y1-18:
        if m<m1: return True
        if m==m1 and d<=d1: return True
    return False
ans="NO"
for p in set(itertools.permutations([a,b,c])):
    d,m,y=p
    if 1<=m<=12 and 1<=d<=31 and ok(d,m,y):
        ans="YES"
        break
print(ans)
--------------------------------------------------------------------
from collections import defaultdict
n=int(input())
g=defaultdict(int),[]
adj=defaultdict(list)
for _ in range(n):
    u,v=map(int, input().split())
    adj[u].append(v)
    adj[v].append(u)
s=0
for k in adj:
    if len(adj[k])==1:
        s=k
        break
res=[s]
while len(res)<=n:
    cur=res[-1]
    for nx in adj[cur]:
        if len(res)==1 or nx!=res[-2]:
            res.append(nx)
            break
print("\n".join(map(str,res)))
--------------------------------------------------------------------
n=int(input())
a=[]
s=set()
for _ in range(n):
    a.append(tuple(map(int, input().split())))
for x,d in a:
    s.add((x,x+d))
ans="NO"
for x,d in a:
    if (x+d,x) in s:
        ans="YES"
        break
print(ans)
--------------------------------------------------------------------
w=int(input())
l=list(map(int,input().split()))
l.sort(reverse=True)
s=0
c=0
for i in range(len(l)):
    if s>=w:
        break
    s+=l[i]
    c+=1
print(c if s>=w else -1)
--------------------------------------------------------------------
n=int(input())
a=list(map(int,input().split()))
s=set(a)
l=list(s)
l.sort()
ans="NO"
for i in range(len(l)-1):
    if 2*l[i]>l[i+1]:
        ans="YES"
        break
print(ans)
--------------------------------------------------------------------
p=int(input())
a=list(map(int,input().split()))
i=0
while True:
    if p<=a[i]:
        print(i+1)
        break
    p-=a[i]
    i=(i+1)%7
----------------------------------*-----------*---------------------
def run():
    try:
        n=int(input())
        a=[input().strip() for _ in range(n)]
        a.sort(key=lambda x: (-x.count('s')/(x.count('h') if x.count('h') else 1)))
        s=""
        for i in a:
            s+=i
        c=0
        sc=0
        for i in s:
            if i=='s':
                sc+=1
            else:
                c+=sc
        print(c)
    except ZeroDivisionError:
        pass

run()
--------------------------------------------------------------------
def run():
    try:
        t=int(input())
        for _ in range(t):
            n,k,d=map(int,input().split())
            a=list(map(int,input().split()))
            ans=n
            for i in range(n-d+1):
                ans=min(ans,len(set(a[i:i+d])))
            print(ans)
    except:
        pass

run()
--------------------------------------------------------------------
def run():
    try:
        n=int(input())
        a=list(map(int,input().split()))
        c=0
        while True:
            m=max(a[1:])
            if a[0]>m:
                print(c)
                break
            i=a[1:].index(m)+1
            a[i]-=1
            a[0]+=1
            c+=1
    except:
        pass

run()
--------------------------------------------------------------------
print(1)
