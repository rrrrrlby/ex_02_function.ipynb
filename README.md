print('Hello python!') #打印字符串
​
Hello python!
print("Hello world!")
print("_"*50)
print("人生很简单，做了决定就不要后悔。")
print("Life is simpleYou make choices and you don't look back.")
​
Hello world!
_________________________________________________
人生很简单，做了决定就不要后悔。
Life is simpleYou make choices and you don't look back.
print("加：",1+0) #打印简单的运算
print("减：",1-1)
print("乘：",1*3)
print("除：",1/3)
print("整除：", 5//2)
print("余数：", 5%2)
print("幂：",4**3)
​
加： 1
减： 0
乘： 3
除： 0.3333333333333333
整除： 2
余数： 1
幂： 64
x=100
monadic_equation=2*x+1
print("monadic_equation=",monadic_equation)
print("monadic_equation=%.2f"%monadic_equation) #%字符串格式化方法
print("monadic_equation={:.2f}".format(monadic_equation)) #format()字符串格式化方法
​
monadic_equation= 201
monadic_equation=201.00
monadic_equation=201.00
city_name="Xi'an"
coordinate_longitude=108.942292
coordiante_latitude=34.261013
print("The longitude of the Xi'an coordinate is {lon:.2f}, and the latitude is {lat}.".format(lon=coordinate_longitude,lat=coordiante_latitude))
​
The longitude of the Xi'an coordinate is 108.94, and the latitude is 34.261013.
x,y,b=1,2,3 #unpacking 序列解包。尝试，x,y,*z=0,1,2,3,4,5,6; x,y,*z=0,1; (x,y),(a,b)=(0,1),(2,3)
func_2=2*x+3*y+b
print("func_2={}".format(x,y,b,func_2))
​
func_2=1
lst_n=list(range(5,20,3)) #建立列表。range(start,stop,[,step])建立区间。
print(lst_n)
print("The list length={}".format(len(lst_n)))
print("Maximum value={}".format(max(lst_n)))
print("Minimum value={}".format(min(lst_n)))
​
[5, 8, 11, 14, 17]
The list length=5
Maximum value=17
Minimum value=5
lst_s=list(map(chr,range(100,110)))
print(lst_s)
print("_"*50)
print("[3:6]->{}".format(lst_s[3:6]))
print("[-3:-1]->{}".format(lst_s[-3:-1]))
print("[-3:]->{}".format(lst_s[-3:]))
print("[:3]->{}".format(lst_s[:3]))
print("[:]->{}".format(lst_s[:]))
​
['d', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm']
__________________________________________________
[3:6]->['g', 'h', 'i']
[-3:-1]->['k', 'l']
[-3:]->['k', 'l', 'm']
[:3]->['d', 'e', 'f']
[:]->['d', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm']
help(map) #用help()方法查看说明
​
Help on class map in module builtins:

class map(object)
 |  map(func, *iterables) --> map object
 |  
 |  Make an iterator that computes the function using arguments from
 |  each of the iterables.  Stops when the shortest iterable is exhausted.
 |  
 |  Methods defined here:
 |  
 |  __getattribute__(self, name, /)
 |      Return getattr(self, name).
 |  
 |  __iter__(self, /)
 |      Implement iter(self).
 |  
 |  __next__(self, /)
 |      Implement next(self).
 |  
 |  __reduce__(...)
 |      Return state information for pickling.
 |  
 |  ----------------------------------------------------------------------
 |  Static methods defined here:
 |  
 |  __new__(*args, **kwargs) from builtins.type
 |      Create and return a new object.  See help(type) for accurate signature.

help(chr)
​
Help on built-in function chr in module builtins:

chr(i, /)
    Return a Unicode string of one character with ordinal i; 0 <= i <= 0x10ffff.

print(lst_s)
print("_"*50)
print("[0:10:2]->{}".format(lst_s[0:10:2]))
print("[::3]->{}".format(lst_s[::3]))
print("[9:3:-2]->{}".format(lst_s[9:3:-2]))
print("[20:3:-2]->{}".format(lst_s[20:3:-2]))
print("[7::-2]->{}".format(lst_s[7::-2]))
print("[:3:-2]->{}".format(lst_s[:3:-2]))
​
['d', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm']
__________________________________________________
[0:10:2]->['d', 'f', 'h', 'j', 'l']
[::3]->['d', 'g', 'j', 'm']
[9:3:-2]->['m', 'k', 'i']
[20:3:-2]->['m', 'k', 'i']
[7::-2]->['k', 'i', 'g', 'e']
[:3:-2]->['m', 'k', 'i']
print(lst_s)
print("_"*50)
lst_s[5]=99 #元素赋值
print("lst_s[5]=99->{}".format(lst_s))
lst_none=lst_s+[None]*6
print("lst_s+[None]*6->{}".format(lst_none))
lst_none[13]=2015
print("lst_none[13]=2015->{}".format(lst_none))
lst_none[-6:-3]=list(range(100,104,2)) #分片赋值
print("lst_none[-6:-3]=list(range(100,104,2))->{}".format(lst_none))
lst_none[1:1]=[0,0,0,12]
print("lst_none[1:1]=[0,0,0,12]->{}".format(lst_none))
del lst_none[-2:] #删除元素
print("del lst_none[-2:]->{}".format(lst_none))
​
['d', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm']
__________________________________________________
lst_s[5]=99->['d', 'e', 'f', 'g', 'h', 99, 'j', 'k', 'l', 'm']
lst_s+[None]*6->['d', 'e', 'f', 'g', 'h', 99, 'j', 'k', 'l', 'm', None, None, None, None, None, None]
lst_none[13]=2015->['d', 'e', 'f', 'g', 'h', 99, 'j', 'k', 'l', 'm', None, None, None, 2015, None, None]
lst_none[-6:-3]=list(range(100,104,2))->['d', 'e', 'f', 'g', 'h', 99, 'j', 'k', 'l', 'm', 100, 102, 2015, None, None]
lst_none[1:1]=[0,0,0,12]->['d', 0, 0, 0, 12, 'e', 'f', 'g', 'h', 99, 'j', 'k', 'l', 'm', 100, 102, 2015, None, None]
del lst_none[-2:]->['d', 0, 0, 0, 12, 'e', 'f', 'g', 'h', 99, 'j', 'k', 'l', 'm', 100, 102, 2015]
lst_s_2=list(map(chr,range(100,105)))
print(lst_s_2)
print("_"*50)
lst_s_2.append(99)
print("lst_s_2.append(99)->{}".format(lst_s_2))
lst_s_2.append(list(range(50,80,5)))
print("lst_s_2.append(list(range(50,80,5)))->{}".format(lst_s_2))
lst_spechars=['*',')','*']
lst_s_2.extend(lst_spechars)
print("lst_s_2.extend(lst_spechars)->{}".format(lst_s_2))
print("lst_s_2.count('*')={}".format(lst_s_2.count('*')))
print("lst_s_2.index('e')={}".format(lst_s_2.index('e')))
lst_s_2.insert(2,[1000,1200,1500])
print("lst_s_2.insert(2,[1000,1200,1500])->{}".format(lst_s_2))
print("lst_s_2.pop(7)_popup->{}".format(lst_s_2.pop(7)))
print("lst_s_2.pop(7)_retention->{}".format(lst_s_2))
lst_s_2.remove('*')
print("lst_s_2.remove('*')_retention->{}".format(lst_s_2))
list_n_2=[2,42,6,95,4,3]
list_n_2.sort()
print("list_n_2.sort()->{}".format(list_n_2))
​
['d', 'e', 'f', 'g', 'h']
__________________________________________________
lst_s_2.append(99)->['d', 'e', 'f', 'g', 'h', 99]
lst_s_2.append(list(range(50,80,5)))->['d', 'e', 'f', 'g', 'h', 99, [50, 55, 60, 65, 70, 75]]
lst_s_2.extend(lst_spechars)->['d', 'e', 'f', 'g', 'h', 99, [50, 55, 60, 65, 70, 75], '*', ')', '*']
lst_s_2.count('*')=2
lst_s_2.index('e')=1
lst_s_2.insert(2,[1000,1200,1500])->['d', 'e', [1000, 1200, 1500], 'f', 'g', 'h', 99, [50, 55, 60, 65, 70, 75], '*', ')', '*']
lst_s_2.pop(7)_popup->[50, 55, 60, 65, 70, 75]
lst_s_2.pop(7)_retention->['d', 'e', [1000, 1200, 1500], 'f', 'g', 'h', 99, '*', ')', '*']
lst_s_2.remove('*')_retention->['d', 'e', [1000, 1200, 1500], 'f', 'g', 'h', 99, ')', '*']
list_n_2.sort()->[2, 3, 4, 6, 42, 95]
tuple_1=2,3,5,
print("tuple_1=2,3,5,->{}".format(tuple_1))
print("3*(20*3,)->{}".format(3*(20*3,)))
print("tuple((5,8,9))->{}".format(tuple((5,8,9)))) #用()
print("tuple([5,8,9])->{}".format(tuple([5,8,9]))) #用[]
​
tuple_1=2,3,5,->(2, 3, 5)
3*(20*3,)->(60, 60, 60)
tuple((5,8,9))->(5, 8, 9)
tuple([5,8,9])->(5, 8, 9)
import random
items=[(0,[i for i in range(5)]),(1,[random.sample(list(range(100,200,1)),3)]),(2,'python')] #[i for i in range(5)] 为列表推导式 list comprehension/derivation
print("items->{}".format(items))
dic=dict(items)
print("dic=dict(items)->{}".format(dic))
print("dic[1]->{}".format(dic[1]))
​
items->[(0, [0, 1, 2, 3, 4]), (1, [[115, 190, 135]]), (2, 'python')]
dic=dict(items)->{0: [0, 1, 2, 3, 4], 1: [[115, 190, 135]], 2: 'python'}
dic[1]->[[115, 190, 135]]
print("len(dic)->{}".format(len(dic)))
dic[3]=(random.random(),random.uniform(200,300))
print("dic[3]=(random.random(),random.uniform(200,300))->{}".format(dic))
del dic[1]
print("del dic[1]->{}".format(dic))
print("3 in dic->{}".format(3 in dic))
print("5 in dic->{}".format(5 in dic))
print("dic.keys()->{}".format(dic.keys())) #应该放在字典的方法一节里
print("dic.values()->{}".format(dic.values()))
print("dic.items()->{}".format(dic.items()))
print("_"*50)
print("list(dic.keys())->{}".format(list(dic.keys())))
​
len(dic)->3
dic[3]=(random.random(),random.uniform(200,300))->{0: [0, 1, 2, 3, 4], 1: [[115, 190, 135]], 2: 'python', 3: (0.4111404575271732, 245.30891046273968)}
del dic[1]->{0: [0, 1, 2, 3, 4], 2: 'python', 3: (0.4111404575271732, 245.30891046273968)}
3 in dic->True
5 in dic->False
dic.keys()->dict_keys([0, 2, 3])
dic.values()->dict_values([[0, 1, 2, 3, 4], 'python', (0.4111404575271732, 245.30891046273968)])
dic.items()->dict_items([(0, [0, 1, 2, 3, 4]), (2, 'python'), (3, (0.4111404575271732, 245.30891046273968))])
__________________________________________________
list(dic.keys())->[0, 2, 3]
for k,v in enumerate(dic.items()): #for循环在后文
    print(k,v)
​
0 (0, [0, 1, 2, 3, 4])
1 (2, 'python')
2 (3, (0.4111404575271732, 245.30891046273968))
lst_A=list(range(6,20,3))
lst_B=list(range(100,150,15))
print("lst_A={},lst_B={}".format(lst_A,lst_B))
dic_2={0:lst_A,1:lst_B}
print("dic_2={}".format(dic_2))
print("_"*50)
dic_assignment=dic_2
print("dic_assignment={}".format(dic_assignment))
dic_2.clear()
print("dic_2.clear()->{}".format(dic_2))
print("dic_assignment={}".format(dic_assignment))
dic_2[5]=list(range(1,9,2))
print("dic_2[5]=list(range(1,9,2))->{}".format(dic_2))
dic_copy=dic_2.copy()
print("dic_copy=dic_2.copy()->{}".format(dic_copy))
dic_2[8]=[5,7]
print("dic_2[8]=[5,7]->{}".format(dic_2))
print("dic_copy={}".format(dic_copy))
dic_copy[5].remove(5)
print("dic_copy[5].remove(5)->{}".format(dic_copy))
dic_copy.setdefault(6,[77,99]) #返回指定键的值，如果不存在该键，则字典增加新的键/值对
print("dic_copy.setdefault(6,[77,99])->{}".format(dic_copy))
dic_2.pop(5) #移除指定键/值，并返回该值
print("dic_2.pop(5)->{}".format(dic_2))
dic_update={8:[5,7,6,3,2],9:[3,2,33,55,66]}
print("dic_update={}".format(dic_update))
dic_2.update(dic_update) #更新字典
print("dic_2.update(dic_update->{}".format(dic_2))
print("dic_2.get(9)->{}".format(dic_2.get(9)))
dic_2.popitem() #随即弹出一对键/值，并在该字典中移除
print("dic_2.popitem()->{}".format(dic_2))
​
dic_3={}.fromkeys([0,1,2,3,4,'A']) #给定键，建立值为空的字典
print("dic_3={}"+".fromkeys([0,1,2,3,4,'A'])->{}".format(dic_3)) #找下escape characters 脱字符
​
lst_A=[6, 9, 12, 15, 18],lst_B=[100, 115, 130, 145]
dic_2={0: [6, 9, 12, 15, 18], 1: [100, 115, 130, 145]}
__________________________________________________
dic_assignment={0: [6, 9, 12, 15, 18], 1: [100, 115, 130, 145]}
dic_2.clear()->{}
dic_assignment={}
dic_2[5]=list(range(1,9,2))->{5: [1, 3, 5, 7]}
dic_copy=dic_2.copy()->{5: [1, 3, 5, 7]}
dic_2[8]=[5,7]->{5: [1, 3, 5, 7], 8: [5, 7]}
dic_copy={5: [1, 3, 5, 7]}
dic_copy[5].remove(5)->{5: [1, 3, 7]}
dic_copy.setdefault(6,[77,99])->{5: [1, 3, 7], 6: [77, 99]}
dic_2.pop(5)->{8: [5, 7]}
dic_update={8: [5, 7, 6, 3, 2], 9: [3, 2, 33, 55, 66]}
dic_2.update(dic_update->{8: [5, 7, 6, 3, 2], 9: [3, 2, 33, 55, 66]}
dic_2.get(9)->[3, 2, 33, 55, 66]
dic_2.popitem()->{8: [5, 7, 6, 3, 2]}
dic_3={}.fromkeys([0,1,2,3,4,'A'])->{0: None, 1: None, 2: None, 3: None, 4: None, 'A': None}
lst_s_3=list("Hello Python!")
print("lst_s_3=list(\"Hello Python!\")->{}".format(lst_s_3)) #"\" escape character
print("\"Hellow\"+\" Python!\"->{}".format("Hellow"+" Python!"))
print("\"+\".join(str(123456))->{}".format("+".join(str(123456))))
print("len(\"Hellow Python!\")->{}".format(len("Hellow Python!")))
coordinates="120.132007,30.300508,9.7"
print("coordinates.split(\",\")->{}".format(coordinates.split(",")))
print("eval(coordinates)->{}".format(eval(coordinates))) #通常用eval()方法将字符串，转换为对应数值形式；
print("\"Hello Python!\".lower()->{}".format("Hello Python!".lower()))
print("\"Hello Python!\".upper()->{}".format("Hello Python!".upper()))
print("\"Hello Python!\"[6:]->{}".format("Hello Python!"[6:]))
print("\"    Hello Python!    \".strip()->{}".format("    Hello Python!    ".strip()))
print("\"Hello Python!\".replace(\"Python\",\"Grasshopper\")->{}".format("Hello Python!".replace("Python","Grasshopper")))
hello_lst=list("Hello Python!")
hello_lst.sort()
print("hello_lst.sort()>{}".format(hello_lst))
print("\"Hello Python!\".find(\"Py\")->{}".format("Hello Python!".find("Py")))
​
lst_s_3=list("Hello Python!")->['H', 'e', 'l', 'l', 'o', ' ', 'P', 'y', 't', 'h', 'o', 'n', '!']
"Hellow"+" Python!"->Hellow Python!
"+".join(str(123456))->1+2+3+4+5+6
len("Hellow Python!")->14
coordinates.split(",")->['120.132007', '30.300508', '9.7']
eval(coordinates)->(120.132007, 30.300508, 9.7)
"Hello Python!".lower()->hello python!
"Hello Python!".upper()->HELLO PYTHON!
"Hello Python!"[6:]->Python!
"    Hello Python!    ".strip()->Hello Python!
"Hello Python!".replace("Python","Grasshopper")->Hello Grasshopper!
hello_lst.sort()>[' ', '!', 'H', 'P', 'e', 'h', 'l', 'l', 'n', 'o', 'o', 't', 'y']
"Hello Python!".find("Py")->6
format_str="Hello,%s and %s!"
values=("Python","Grasshopper")
new_str=format_str % values
print("new_str=format_str % values->{}".format(new_str))
​
format_str_2="Pi with three decimals:%.3f,and enter a value with percent sign:%.2f %%" #如果字符串里包含实际的%，则通过%%即两个百分号进行转义
​
from math import pi
new_str_2=format_str_2 % (pi,3.1415926)
print("new_str_2=format_str_2 % (pi,3.1415926)->{}".format(new_str_2))
​
new_str=format_str % values->Hello,Python and Grasshopper!
new_str_2=format_str_2 % (pi,3.1415926)->Pi with three decimals:3.142,and enter a value with percent sign:3.14 %
format_str_3="%10f,%10.2f,%.2f,%.5s,%.*s,%d,%x,%f"
new_str_3=format_str_3%(pi,pi,pi,"Hello Python!",5,"Hello Python!",52,52,pi)
print("{}".format(new_str_3))
​
  3.141593,      3.14,3.14,Hello,Hello,52,34,3.141593
from string import Template
s_template_1=Template("$x,glorious,$x!")
s_1=s_template_1.substitute(x="Python")
print("s_1=s_template_1.substitute(x=\"Python\")->{}".format(s_1))
s_template_2=Template("${x}thon is amazing!")
s_2=s_template_2.substitute(x="py")
print("s_2=s_template_2.substitute(x=\"py\")->{}".format(s_2))
s_template_3=Template("$x and $y are both amazing!")
substitute_dict=dict([('x','Python'),('y','Grasshopper')])
print("substitute_dict={}".format(substitute_dict))
s_3=s_template_3.substitute(substitute_dict)
print("s_3=s_template_3.substitute(substitute_dict)->{}".format(s_3))
​
s_1=s_template_1.substitute(x="Python")->Python,glorious,Python!
s_2=s_template_2.substitute(x="py")->python is amazing!
substitute_dict={'x': 'Python', 'y': 'Grasshopper'}
s_3=s_template_3.substitute(substitute_dict)->Python and Grasshopper are both amazing!
import re
pattern_1='Python'
text="Hello Python!"
print("re.findall(pattern_1,text)->{}".format(re.findall(pattern_1,text)))
pattern_2='python'
print("re.findall(pattern_2,text)->{}".format(re.findall(pattern_2,text)))
​
re.findall(pattern_1,text)->['Python']
re.findall(pattern_2,text)->[]
print("re.findall('.ython','Hello Python!')->{}".format(re.findall('.ython','Hello Python!')))
print("re.findall('.ython','Hello gython!')->{}".format(re.findall('.ython','Hello gython!')))
print("re.findall('.ython','Hello gPython!')->{}".format(re.findall('.ython','Hello gPython!')))
print("re.findall('.ython','Hello Pthon!')->{}".format(re.findall('.ython','Hello Pthon!')))
​
re.findall('.ython','Hello Python!')->['Python']
re.findall('.ython','Hello gython!')->['gython']
re.findall('.ython','Hello gPython!')->['Python']
re.findall('.ython','Hello Pthon!')->[]
print("re.findall(r'w?cadesign\.cn,w+\.cadesign\.cn','cadesign.cn,www.cadesign.cn')->{}".format(re.findall(r'w?cadesign\.cn,w+\.cadesign\.cn','cadesign.cn,www.cadesign.cn')))
print("re.findall(r'w{2}"+"\.cadesign\.cn','www.cadesign.cn')->{}".format(re.findall(r'w{2}\.cadesign\.cn','www.cadesign.cn')))
print("re.findall(r'w{1,3}"+"\.cadesign\.cn','www.cadesign.cn')->{}".format(re.findall(r'w{1,3}\.cadesign\.cn','www.cadesign.cn')))
​
re.findall(r'w?cadesign\.cn,w+\.cadesign\.cn','cadesign.cn,www.cadesign.cn')->['cadesign.cn,www.cadesign.cn']
re.findall(r'w{2}\.cadesign\.cn','www.cadesign.cn')->['ww.cadesign.cn']
re.findall(r'w{1,3}\.cadesign\.cn','www.cadesign.cn')->['www.cadesign.cn']
print("re.findall('[Py]*thon!','Hello Python!')->{}".format(re.findall('[Py]*thon!','Hello Python!')))
print("re.findall('[Py]*thon!','Hello Pthon!')->{}".format(re.findall('[Py]*thon!','Hello Pthon!')))
print("re.findall('[Py]*thon!','Hello ython!')->{}".format(re.findall('[Py]*thon!','Hello ython!')))
print("re.findall('[Py]*thon!','Hello ython!')->{}".format(re.findall('[Py]*thon!','Hello thon!')))
​
re.findall('[Py]*thon!','Hello Python!')->['Python!']
re.findall('[Py]*thon!','Hello Pthon!')->['Pthon!']
re.findall('[Py]*thon!','Hello ython!')->['ython!']
re.findall('[Py]*thon!','Hello ython!')->['thon!']
print("re.findall('python|grasshopper','python')->{}".format(re.findall('python|grasshopper','python')))
print("re.findall('python|grasshopper','grasshopper')->{}".format(re.findall('python|grasshopper','grasshopper')))
print("re.findall('python|grasshopper','grasshopper and python')->{}".format(re.findall('python|grasshopper','grasshopper and python')))
​
re.findall('python|grasshopper','python')->['python']
re.findall('python|grasshopper','grasshopper')->['grasshopper']
re.findall('python|grasshopper','grasshopper and python')->['grasshopper', 'python']
print("re.findall('\d','number=10')->{}".format(re.findall('\d','number=10')))
print("re.findall('\D','number=10')->{}".format(re.findall('\D','number=10')))
print("re.findall('[^0-9]','number=10')->{}".format(re.findall('[^0-9]','number=10')))
print("re.findall('[a-z]','python')->{}".format(re.findall('[a-z]','python-3.0')))
print("re.search('[a-z]+','python')->{}".format(re.search('[a-z]+','python')))
if re.search('[a-z]+','python'):
    print("re.search('[a-z]+','python')->found it!")
print("re.split(',','Hello,,,,,,Python!')->{}".format(re.split(',','Hello,,,,,,Python!')))
print("re.sub('Python','Grasshopper','Hello Python!')->{}".format(re.sub('Python','Grasshopper','Hello Python!')))
​
pattern_compile=re.compile('Python')
print("pattern_compile.findall('Hello,,,,,,Python!')->{}".format(pattern_compile.findall('Hello,,,,,,Python!')))
​
if re.match('p','python'):
    print("re.match('p','python')->found it!")
​
re.findall('\d','number=10')->['1', '0']
re.findall('\D','number=10')->['n', 'u', 'm', 'b', 'e', 'r', '=']
re.findall('[^0-9]','number=10')->['n', 'u', 'm', 'b', 'e', 'r', '=']
re.findall('[a-z]','python')->['p', 'y', 't', 'h', 'o', 'n']
re.search('[a-z]+','python')-><re.Match object; span=(0, 6), match='python'>
re.search('[a-z]+','python')->found it!
re.split(',','Hello,,,,,,Python!')->['Hello', '', '', '', '', '', 'Python!']
re.sub('Python','Grasshopper','Hello Python!')->Hello Grasshopper!
pattern_compile.findall('Hello,,,,,,Python!')->['Python']
re.match('p','python')->found it!
print("\'python\'.find(\'python\')->{}".format('python'.find('python')))
print("\'python\'.find(\'thon\')->{}".format('python'.find('thon')))
print("\'python\'.find(\'a\')->{}".format('python'.find('a')))
print("\'p\' in \'python\'->{}".format('p' in 'python'))
​
'python'.find('python')->0
'python'.find('thon')->2
'python'.find('a')->-1
'p' in 'python'->True
print("\'Hello,,,,,,Python!\'.split(',')->{}".format( 'Hello,,,,,,Python!'.split(',')))
print("\'Hello Python!\'.replace(\'Python\',\'Grasshopper\')->{}".format( 'Hello Python!'.replace('Python','Grasshopper')))
​
'Hello,,,,,,Python!'.split(',')->['Hello', '', '', '', '', '', 'Python!']
'Hello Python!'.replace('Python','Grasshopper')->Hello Grasshopper!
match_1=re.match(r'www\.(.*)\..{3}','www.python.org')
print("match_1.gourp(1)->{}".format(match_1.group(1)))
print("match_1.start(1)->{}".format(match_1.start(1)))
print("match_1.end(1)->{}".format(match_1.end(1)))
print("match_1.span(1)->{}".format(match_1.span(1)))
match_2=re.match(r'www\.(.*)\.(.{3})','www.python.org')
print("match_2.group(1)->{}".format(match_2.group(1)))
print("match_2.group(2)->{}".format(match_2.group(2)))
​
match_1.gourp(1)->python
match_1.start(1)->4
match_1.end(1)->10
match_1.span(1)->(4, 10)
match_2.group(1)->python
match_2.group(2)->org
lst_1=list(range(29,37,2))
print("lst_1={}".format(lst_1))
print("_"*50)
print("for i in lst_1:")
for i in lst_1:
    print(i)
print("for i in range(len(lst_1)):")
for i in range(len(lst_1)):
    print("idx={},val={}".format(i,lst_1[i]))
print("+"*50)   
dic_4=dict(a=2,b=3,c=6,d=0)
print("dic_4={}".format(dic_4))
print("_"*50)
print("for k in dic_4:")
for k in dic_4:
    print(k)
print("for k,v in dic_4.items():")
for k,v in dic_4.items():
    print("key={},val={}".format(k,v))
​
lst_1=[29, 31, 33, 35]
__________________________________________________
for i in lst_1:
29
31
33
35
for i in range(len(lst_1)):
idx=0,val=29
idx=1,val=31
idx=2,val=33
idx=3,val=35
++++++++++++++++++++++++++++++++++++++++++++++++++
dic_4={'a': 2, 'b': 3, 'c': 6, 'd': 0}
__________________________________________________
for k in dic_4:
a
b
c
d
for k,v in dic_4.items():
key=a,val=2
key=b,val=3
key=c,val=6
key=d,val=0
x=1
while x<=100:
    print("x={}".format(x))
    x+=10 #增量赋值; x*=2     
​
x=1
x=11
x=21
x=31
x=41
x=51
x=61
x=71
x=81
x=91
x=1
while x<=100:
    print("x={}".format(x))
    x+=10 
    if x>=50:break    
    
import sys
print("sys.maxsize={}".format(sys.maxsize))
for i in range(sys.maxsize):
    print("i={}".format(i))  #?
    i+=10
    if i>=30:break
​
x=1
x=11
x=21
x=31
x=41
sys.maxsize=9223372036854775807
i=0
i=1
i=2
i=3
i=4
i=5
i=6
i=7
i=8
i=9
i=10
i=11
i=12
i=13
i=14
i=15
i=16
i=17
i=18
i=19
i=20
sum = 0
​
x = 1
​
n = 1
​
while True:
​
    if n > 20:
​
        break
​
    sum = sum + x
​
    x = x * 2
​
    n = n + 1 
​
print(sum)
1048575
lst_a=[0,1,2,3]
lst_b=['point_a','point_b','point_c','point_d']
zip_lst=zip(lst_a,lst_b) #The zip() function takes iterables (can be zero or more), aggregates them in a tuple, and returns it.
print("zip_lst=zip(lst_a,lst_b)->{}".format(zip_lst))
print("dict(zip_lst)->{}".format(dict(zip_lst)))
​
zip_lst=zip(lst_a,lst_b) #迭代对象临时存储，读取完后为空
for a,b in zip_lst:
    print(a,b)
    
zip_lst=zip(lst_a,lst_b)
a,b=zip(*zip_lst)
print("a={},b={}".format(a,b))
​
zip_lst=zip(lst_a,lst_b)-><zip object at 0x0000012B36079380>
dict(zip_lst)->{0: 'point_a', 1: 'point_b', 2: 'point_c', 3: 'point_d'}
0 point_a
1 point_b
2 point_c
3 point_d
a=(0, 1, 2, 3),b=('point_a', 'point_b', 'point_c', 'point_d')
lst_c=['point_a','point_b','point_c','point_d']
dic_4={}
for idx,value in enumerate(lst_c):
    dic_4[idx]=value
print("dic_4={}".format(dic_4))
print("dict((i,v) for i,v in enumerate(lst_c))->{}".format(dict((i,v) for i,v in enumerate(lst_c)))) #list comprehension
print("_"*50)
for i,(a,b) in enumerate(zip(lst_a,lst_b)):
    print('%d:%s,%s'%(i,a,b))
​
dic_4={0: 'point_a', 1: 'point_b', 2: 'point_c', 3: 'point_d'}
dict((i,v) for i,v in enumerate(lst_c))->{0: 'point_a', 1: 'point_b', 2: 'point_c', 3: 'point_d'}
__________________________________________________
0:0,point_a
1:1,point_b
2:2,point_c
3:3,point_d
print("[x*x for x in range(3,37,5) if x%2==0]->{}".format([x*x for x in range(3,37,5) if x%2==0]))
print("[(x,y) for x in range(3)for y in range(2)]->{}".format([(x,y) for x in range(3)for y in range(2)]))
print("[(x,y) for x,y in zip(range(3),range(2))]->{}".format([(x,y) for x,y in zip(range(3),range(2))]))
nested_list=[[a for a in range(1,10,3)],2,3,[b for b in range(60,100,7)],[[c for c in range(1000,2000,120)],3,9]]
print("[[a for a in range(1,10,3)],2,3,[b for b in range(60,100,7)],[[c for c in range(1000,2000,120)],3,9]]->{}".format(nested_list)) #嵌套列表推导式
​
flatten_lst=lambda lst: [m for n_lst in lst for m in flatten_lst(n_lst)] if type(lst) is list else [lst] #展平列表常用，可以放置到单独的.py文件中调用。lambda函数后文阐述
print("flatten_lst(nested_list)->{}".format(flatten_lst(nested_list)))
​
[x*x for x in range(3,37,5) if x%2==0]->[64, 324, 784]
[(x,y) for x in range(3)for y in range(2)]->[(0, 0), (0, 1), (1, 0), (1, 1), (2, 0), (2, 1)]
[(x,y) for x,y in zip(range(3),range(2))]->[(0, 0), (1, 1)]
[[a for a in range(1,10,3)],2,3,[b for b in range(60,100,7)],[[c for c in range(1000,2000,120)],3,9]]->[[1, 4, 7], 2, 3, [60, 67, 74, 81, 88, 95], [[1000, 1120, 1240, 1360, 1480, 1600, 1720, 1840, 1960], 3, 9]]
flatten_lst(nested_list)->[1, 4, 7, 2, 3, 60, 67, 74, 81, 88, 95, 1000, 1120, 1240, 1360, 1480, 1600, 1720, 1840, 1960, 3, 9]
   x=10
if x<0:
    print('It is negative.')
elif x==0:
    print('Equal to zero.')
elif 0<x<10:
    print('Positive but smaller than 10')
else:
    print('Positive and larger than or equal to 10.')
​
​
Positive and larger than or equal to 10.
x=y=[3,6,9]
z=[3,6,9]
print("x==y->{}".format(x==y))
print("x is y->{}".format(x is y))
print("x==z->{}".format(x==z))
print("x is z->{}".format(x is z))
print("x is not y->{}".format(x is not y))
print("x is not z->{}".format(x is not z))
print("id_x:{};id_y:{};id_z:{}".format(id(x),id(y),id(z))) #Memory Location
​
del x[2]
print("x={},y={},z={} after del x[2]".format(x,y,z))
​
x==y->True
x is y->True
x==z->True
x is z->False
x is not y->False
x is not z->True
id_x:1285101800448;id_y:1285101800448;id_z:1285101798592
x=[3, 6],y=[3, 6],z=[3, 6, 9] after del x[2]
x=[3,6,9]
print("3 in x->{}".format(3 in x))
print("0 in x->{}".format(0 in x))
print("3 not in x->{}".format(3 not in x))
print("0 not in x->{}".format(0 not in x))
​
3 in x->True
0 in x->False
3 not in x->False
0 not in x->True
a,b,c=0,10,15
if c>a and c<b:
    print('a<c<b')
else: print('a<c<b kidding!!!')
​
a<c<b kidding!!!
def function(arguments):
    statement
    ...
    return values
​
def simple_func(x,y):
    z=pow(x,2)+y
    return z
​
print("simple_func(3,7)->{}".format(simple_func(3,7)))
print("simple_func(7,3)->{}".format(simple_func(7,3)))
print("simple_func(y=7,x=3)->{}".format(simple_func(y=7,x=3)))
​
simple_func(3,7)->16
simple_func(7,3)->52
simple_func(y=7,x=3)->16
def fibonacci(s,count): #定义fib函数的方法较笨
    fib_lst=[0,1]
    fib_part=[]
    if s==0 or s==1:
        fib_part[:]=fib_lst
        for i in range(count-2):
            fib_part.append(fib_part[-1]+fib_part[-2])
    else:
        while True:
            fib_lst[:]=[fib_lst[1],fib_lst[0]+fib_lst[1]]
            #print(fib_lst)
            if fib_lst[1]-s>=0:break
        fib_part[:]=fib_lst
        if abs(fib_lst[0]-s)>=abs(fib_lst[1]-s):
            for i in range(count-1):
                fib_part.append(fib_part[-1]+fib_part[-2])
            fib_part.pop(0)
        else:
            for i in range(count-2):
                fib_part.append(fib_part[-1]+fib_part[-2])
    return fib_part
​
print("fibonacci(6,9)->{}".format(fibonacci(6,9)))
print("fibonacci(7,9)->{}".format(fibonacci(7,9)))
​
fibonacci(6,9)->[5, 8, 13, 21, 34, 55, 89, 144, 233]
fibonacci(7,9)->[8, 13, 21, 34, 55, 89, 144, 233, 377]
def factorial(n):
    if n==1:
        return 1
    else:
        return n*factorial(n-1)
print(factorial(7))
​
5040
class Bird:
    fly='Whirring' #美 /wɜːr/ 
    def __init__(self):
        self.hungry=True
    def eat(self):
        if self.hungry:
            print('Aaaah...')
            self.hungry=False
        else:
            print('No.Thanks!')
​
class Apodidae(Bird):  #/'æpədədi:/
    def __init__(self):
        super(Apodidae,self).__init__()
        self.sound='Squawk!' #美 /skwɔːk/ 
    def sing(self):
        print(self.sound)
​
swift=Apodidae()
print("swift.fly->{}".format(swift.fly))
print("swift.eat()->")
swift.eat()
print("swift.eat()->")
swift.eat()
print("swift.sing()->")
swift.sing()
​
swift.fly->Whirring
swift.eat()->
Aaaah...
swift.eat()->
No.Thanks!
swift.sing()->
Squawk!
blackswift=Apodidae()
scarceswift=Apodidae()
print("blackswift.sing()->")
blackswift.sing()
print("scarceswift.sing()->")
scarceswift.sing()
​
blackswift.sing()->
Squawk!
scarceswift.sing()->
Squawk!
print("blackswift.fly->{}".format(blackswift.fly))
blackswift.fly='humming' #重新赋予实例的属性
print("blackswift.fly after redefining the blackswif's attribute->{}".format(blackswift.fly))
print("scarceswift.fly->{}".format(scarceswift.fly))
​
blackswift.fly->Whirring
blackswift.fly after redefining the blackswif's attribute->humming
scarceswift.fly->Whirring
blackswift.sing()
​
Squawk!
help(Bird)
​
Help on class Bird in module __main__:

class Bird(builtins.object)
 |  Methods defined here:
 |  
 |  __init__(self)
 |      Initialize self.  See help(type(self)) for accurate signature.
 |  
 |  eat(self)
 |  
 |  ----------------------------------------------------------------------
 |  Data descriptors defined here:
 |  
 |  __dict__
 |      dictionary for instance variables (if defined)
 |  
 |  __weakref__
 |      list of weak references to the object (if defined)
 |  
 |  ----------------------------------------------------------------------
 |  Data and other attributes defined here:
 |  
 |  fly = 'Whirring'

help(Apodidae)
​
Help on class Apodidae in module __main__:

class Apodidae(Bird)
 |  Method resolution order:
 |      Apodidae
 |      Bird
 |      builtins.object
 |  
 |  Methods defined here:
 |  
 |  __init__(self)
 |      Initialize self.  See help(type(self)) for accurate signature.
 |  
 |  sing(self)
 |  
 |  ----------------------------------------------------------------------
 |  Methods inherited from Bird:
 |  
 |  eat(self)
 |  
 |  ----------------------------------------------------------------------
 |  Data descriptors inherited from Bird:
 |  
 |  __dict__
 |      dictionary for instance variables (if defined)
 |  
 |  __weakref__
 |      list of weak references to the object (if defined)
 |  
 |  ----------------------------------------------------------------------
 |  Data and other attributes inherited from Bird:
 |  
 |  fly = 'Whirring'

class Fibs():
    def __init__(self):
        self.a=0
        self.b=1
    def next(self):  #实现迭代器的next方法
        self.a,self.b=self.b,self.a+self.b
        return self.a
    def __iter__(self): #实现迭代方法
        return self
​
f=Fibs()
fa=[]
fb=[]
for i in range(9):
    fa.append(f.next())
print("fa={}".format(fa))
for i in range(5):
    fb.append(f.next())
print("fb={}".format(fb))
​
fa=[1, 1, 2, 3, 5, 8, 13, 21, 34]
fb=[55, 89, 144, 233, 377]
lst_e=[list(range(3,20,3)),[3,7,67,list(range(5)),89]]
print("lst_e={}".format(lst_e))
print("_"*50)
flatten_lst=[]
for v_1 in lst_e:
    try:
        for v_2 in v_1:
            try:
                for v_3 in v_2:
                    flatten_lst.append(v_3)
            except TypeError:
                flatten_lst.append(v_2)
    except TypeError:
        flatten_lst.append(v_1)
print("flatten_lst={}".format(flatten_lst))
​
lst_e=[[3, 6, 9, 12, 15, 18], [3, 7, 67, [0, 1, 2, 3, 4], 89]]
__________________________________________________
flatten_lst=[3, 6, 9, 12, 15, 18, 3, 7, 67, 0, 1, 2, 3, 4, 89]
def flatten(lst): #定义生成器（包含yield语句的函数）
    try: #使用语句try\except捕捉异常        
        for n_lst in lst:  #循环列表            
            for m in flatten(n_lst): #使用递归的方法循环子列表                
                yield m  #使用yield语句，每次产生多个值，当返回一个值时函数就会被冻结，当再次激活时，从停止的那点开始执行
    except TypeError:  #当函数被告知展开一个元素时，引发TypeError异常，生成器返回一个值
        yield lst #生成器返回引发异常的一个值        
​
print("list(flatten(lst_e))->{}".format(list(flatten(lst_e))))
​
list(flatten(lst_e))->[3, 6, 9, 12, 15, 18, 3, 7, 67, 0, 1, 2, 3, 4, 89]
flatten_lst=lambda lst:[m for n_lst in lst for m in flatten_lst(n_lst)] if type(lst) is list else [lst] #lambda 生成器方法
​
def infinite():
    n=0
    while True:
        yield 'num#'+str(n)
        n+=1
​
n=infinite()
print("next(n)->{}".format(next(n)))
print("next(n)->{}".format(next(n)))
print("next(n)->{}".format(next(n)))
print("[next(n) for i in range(5)]->{}".format([next(n) for i in range(5)]))
​
next(n)->num#0
next(n)->num#1
next(n)->num#2
[next(n) for i in range(5)]->['num#3', 'num#4', 'num#5', 'num#6', 'num#7']
n=3
print("[[(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n)]->{}".format([[(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n)]))
print("_"*50)
print("([(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n))->{}".format(([(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n))))
gen=([(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n))
print("next(gen)->{}".format(next(gen)))
print("next(gen)->{}".format(next(gen)))
​
[[(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n)]->[[(-6.283185307179586, -6.283185307179586), (0.0, -6.283185307179586), (6.283185307179586, -6.283185307179586)], [(-6.283185307179586, 0.0), (0.0, 0.0), (6.283185307179586, 0.0)], [(-6.283185307179586, 6.283185307179586), (0.0, 6.283185307179586), (6.283185307179586, 6.283185307179586)]]
__________________________________________________
([(2*pi*(2*(u/(n-1))-1),2*pi*(2*(v/(n-1))-1)) for u in range(n)] for v in range(n))-><generator object <genexpr> at 0x0000012B3608D350>
next(gen)->[(-6.283185307179586, -6.283185307179586), (0.0, -6.283185307179586), (6.283185307179586, -6.283185307179586)]
next(gen)->[(-6.283185307179586, 0.0), (0.0, 0.0), (6.283185307179586, 0.0)]
def f_convert_a(x):
    try:
        return float(x)
    except:
        return x
print("f_convert_a('3.1415')->{}".format(f_convert_a('3.1415')))    
print("f_convert_a('string')->{}".format(f_convert_a('string')))  
print("f_convert_a(3,6,7)->{}".format(f_convert_a((3,6,7))))  
​
f_convert_a('3.1415')->3.1415
f_convert_a('string')->string
f_convert_a(3,6,7)->(3, 6, 7)
def f_convert_c(x):
    try:
        return float(x)
    except ValueError:
        return x
    except TypeError:
        print(x,'TypeError')
print("f_convert_c('3.1415')->{}".format(f_convert_c('3.1415')))    
print("f_convert_c('string')->{}".format(f_convert_c('string')))  
print("f_convert_c(3,6,7)->{}".format(f_convert_c((3,6,7))))         
​
f_convert_c('3.1415')->3.1415
f_convert_c('string')->string
(3, 6, 7) TypeError
f_convert_c(3,6,7)->None
def f_convert_d(x):
    try:
        return float(x)
    except (ValueError,TypeError):
        print(x,'ValueError or TypeError')
print("f_convert_d('3.1415')->{}".format(f_convert_d('3.1415')))    
print("f_convert_d('string')->{}".format(f_convert_d('string')))  
print("f_convert_d(3,6,7)->{}".format(f_convert_d((3,6,7)))) 
​
​
f_convert_d('3.1415')->3.1415
string ValueError or TypeError
f_convert_d('string')->None
(3, 6, 7) ValueError or TypeError
f_convert_d(3,6,7)->None
def f_convert_e(x):
    try:
        return float(x)
    except (ValueError,TypeError) as e:
        return print(x,e)
print("f_convert_e('3.1415')->{}".format(f_convert_e('3.1415')))    
print("f_convert_e('string')->{}".format(f_convert_e('string')))  
print("f_convert_e(3,6,7)->{}".format(f_convert_e((3,6,7))))    
​
f_convert_e('3.1415')->3.1415
string could not convert string to float: 'string'
f_convert_e('string')->None
(3, 6, 7) float() argument must be a string or a number, not 'tuple'
f_convert_e(3,6,7)->None
def f_convert_f(x):
    try:
        return float(x)
    except (ValueError,TypeError) as e:
        pass
print("f_convert_f('3.1415')->{}".format(f_convert_f('3.1415')))    
print("f_convert_f('string')->{}".format(f_convert_f('string')))  
print("f_convert_f(3,6,7)->{}".format(f_convert_f((3,6,7))))     
​
f_convert_f('3.1415')->3.1415
f_convert_f('string')->None
f_convert_f(3,6,7)->None
def f_open_a(fp):
    try:
        f=open(fp,'r')
    except IOError as e:
        print('Unable to open',fp,':%s\n' %e)
    else:
        data=f.read()
        f.close
        return data
tryException_content=f_open_a("./data/tryException.txt")   
print("tryException_content->{}".format(tryException_content))
f_open_a("./data/tryException_.txt")
​
Unable to open ./data/tryException.txt :[Errno 2] No such file or directory: './data/tryException.txt'

tryException_content->None
Unable to open ./data/tryException_.txt :[Errno 2] No such file or directory: './data/tryException_.txt'

def f_open_b(fp):
    try:
        f=open(fp,'r')
    except IOError as e:
        print('Unable to open',fp,':%s\n' %e)
    else:
        data=f.read()
        f.close()
        return data
    finally:
        print('done!')
f_open_b("./data/tryException.txt")        
​
​
Unable to open ./data/tryException.txt :[Errno 2] No such file or directory: './data/tryException.txt'

done!

