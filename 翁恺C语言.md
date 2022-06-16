# 百科园

## 选择题

### 6

> 共15题。(其中有一题重复，已删除)

下面能正确进行字符串赋值操作的是( )

- [ ] `char s[5]={"ABCDE"};`
- [ ] `char *s; scanf("%s",s) ;`
- [x] `char *s ; s="ABCDE" ;`
- [ ] `char s[5]={'A','B','C','D','E'};`

已有函数max(a,b)，为了让函数指针变量p指向函数max，正确的赋值方法是(  )。

- [ ] `*p=max;`
- [ ] `p=max(a,b);`
- [x] `p=max;`
- [ ] `*p=max(a,b);`

若有定义:int (*p)[4];则标识符p(  )。

- [x] 是一个指针，它指向一个含有四个整型元素的一维数组
- [ ] 定义不合法
- [ ] 是一个指向整型变量的指针
- [ ] 是一个指针数组名

下面程序段的运行结果是（  ）。

```c
char a[ ]=”language” , *p ;
p=a ; 
while (*p!='u') { printf(“%c”,*p-32); p++ ; }
```

- [ ] langUAGE
- [ ] LANGUAGE
- [x] LANG
- [ ] language

若要对a进行自增运算，则a应具有下面说明(  )。

- [ ] `char (*a)[3]`
- [ ] `char *a[ ]={"12","ab"};`
- [ ] `int a[3][2];`
- [x] `int b[10], *a=b;`

设p1和p2是指向同一个字符串的指针变量，c为字符变量，则以下能正确执行并得到有意义的结果的赋值语句是(  )。

- [ ] `c=*p1+*p2;`
- [x] `p1=p2;`
- [ ] `c=*p1*(*p2);`
- [ ] `p2=c;`

若有说明：int *p1, *p2,m=5,n;以下均是正确赋值语句的选项是( )。

- [ ] `p1=&m; p2=&p1 ;`
- [ ] `p1=&m; *p1=*p2 ;`
- [ ] `p1=&m; p2=&n; *p1=*p2 ;`
- [x] `p1=&m; p2=p1 ;`

下面程序段的运行结果是( )。

```c
char *s=”abcde” ;
s+=2 ; printf(“%s”,s);
```

- [x] `cde`
- [ ] `字符'c'`
- [ ] `不确定`
- [ ] `字符'c'的地址`

下面判断正确的是（）。

- [ ] `char *a="china"; 等价于 char *a; *a="china" ;`
- [ ] `char c[4]="abc",d[4]="abc"; 等价于 char c[4]=d[4]="abc" ;`
- [x] `char *s="china"; 等价于 char *s; s="china" ;`
- [ ] `char str[10]={"china"}; 等价于 char str[10]; str[ ]={"china";}`

设有程序段:`char s[ ]="china"; char *p ; p=s ;`则下面叙述正确的是（）。

- [ ] `s和p完全相同`
- [ ] `s数组长度和p所指向的字符串长度相等`
- [ ] `数组s中的内容和指针变量p中的内容相等`
- [x] `*p与s[0]相等`

已有定义`int k=2;int *ptr1,*ptr2;`且ptr1和ptr2均已指向变量k，下面不能正确执行的赋值语句是( )

- [ ] `k=*ptr1*(*ptr2);`
- [ ] `k=*ptr1+*ptr2;`
- [ ] `ptr1=ptr2;`
- [x] `ptr2=k;`

若有说明：int *p,m=5,n;以下程序段正确的是( )

- [ ] `p=&n ;scanf("%d",&p);`
- [ ] `scanf("%d",&n); *p=n ;`

> 这个不正确属实离谱！
>
> ```c
> #include <stdio.h>
> int main()
> {
>  int *p,m=5,n;
>  scanf("%d",&n);
>  *p=n ;
>  printf("%d",*p);
>  return 0;
> }
> ```
>
> ```
> 10
> 
> ```
>
> 竟然没能成功输出！

- [ ] `p = &n ;scanf("%d",*p);`
- [x] `p = &n ; *p = m ;`

已有变量定义和函数调用语句：`int a=25;print_value(&a);`下面函数的输出结果是( )

```c
void print_value(int *x)
{ printf(“%d\n”,++*x); }
```

- [x] `26`
- [ ] `25`
- [ ] `24`
- [ ] `23`

变量的指针，其含义是指该变量的( )

- [ ] `名`
- [x] `地址`
- [ ] `一个标志`
- [ ] `值`



### 7

```c
若有定义
#define N 2
#define Y(n) ((N+1)*n)
   则执行语句z=2*(N+Y(5));后，z的值为（   ）。
```

- [ ] `70`
- [x] `34`
- [ ] `语句有错误`

- [ ] `无确定值`

```c
以下程序的运行结果是（  ）。
#include<stdio.h>
#define MIN(x,y) (x)>(y) ? (x) : (y)
int main ( ) {
  int i=10, j=15 , k;
   k = 10*MIN(i,j);
   printf(“%d\n”,k); 
return 0;
}
```

- [ ] `100`
- [x] `10`
- [ ] `150`
- [ ] `15`

```c
以下程序的运行结果是（  ）。
#include<stdio.h>
#define ADD(x) x+x
int main ( )
{
 int m=1,n=2,k=3,sum ; 
   sum = ADD(m+n)*k ;
   printf(“%d\n”,sum) ;
   return 0;
}
```

- [x] `10`

- [ ] `12`
- [ ] `9`
- [ ] `18`

```c
以下程序的运行结果是（   ）。
#include<stdio.h>
#define DOUBLE(r) r*r
int main ( ) {
   int x=1,y=2,t;
   t = DOUBLE(x+y) ;
  printf (“%d\n”,t); return 0;
}
```

- [x] `5`

- [ ] `6`

- [ ] `8`
- [ ] `7`

```c
以下程序的运行结果是（   ）。
#include<stdio.h>
#define X 5
#define Y X+1
#define Z Y*X/2
int main ( ) {
 int a=Y;
 printf(“%d\n”,Z);
 printf(“%d\n”,--a);
return 0;
}
```

- [ ] ```
  12
  6
  ```

- [ ] ```
  12
  5
  ```

- [ ] ```
  7
  6
  ```

- [x] ```
  7
  5
  ```

在“文件包含”预处理命令形式中，当#include后面的文件名用””（双引号）括起时，寻找被包含文件的方式是（  ）。

- [x] `先在源程序所在目录中搜索，再按系统设定的标准方式搜索`

- [ ] `直接按系统设定的标准方式搜索目录`

- [ ] `仅仅搜索当前目录`
- [ ] `仅仅搜索源程序所在目录`

在宏定义#define PI 3.1415926中，用宏名PI代替一个（ ）。

- [ ] `常量`
- [ ] `单精度数`

- [x] `字符串`

- [ ] `双精度数`

以下叙述不正确的是（  ）。

- [ ] `预处理命令行可以出现在C程序中任意一行上`
- [ ] `预处理命令行都必须以＃开始`
- [ ] `在程序中凡是以＃开始的语句行都是预处理命令行`

- [x] `C程序在执行过程中对预处理命令行进行处理`

以下叙述中正确的是（ ）。

- [ ] `在程序的一行上可以出现多个有效的预处理命令行`
- [ ] `使用带参数的宏时，参数的类型应与宏定义时的一致`
- [ ] `C语言的编译预处理就是对源程序进行初步的语法检查`
- [x] `宏替换不占用运行时间，只占用预编译时间`

以下有关宏替换的叙述不正确的是（  ）。

- [ ] `宏替换只是字符串替换`

- [ ] `宏替换不占用运行时间`

- [ ] `宏名无类型`

- [x] `宏名必须用大写字母表示`

在任何情况下计算平方数都不会引起二义性的宏定义是（  ）

- [ ] `#define POWER(x) x*x`

- [x] `#define POWER(x) ((x)*(x))`

- [ ] `#define POWER(x) (x*x)`

- [ ] `#define POWER(x) (x)*(x)`



### 8

```c
以下叙述中正确的是（）
若有以下语句
　　typedefstruct  S
　　｛int g; char h;｝T;
```

- [ ] `S是struct类型的变量`
- [ ] `T是struct S类型的变量`
- [ ] `可用S定义结构体变量`
- [x] `可用T定义结构体变量`

```c
若有以下定义：
struct link
{
int data;
struct link *next;
}a,b,c,*p,*q;
且变量a和b之间已有如下图所示的链表结构，若指针p指向a，指针q指向c。
则能把c插入到a和b之间形成新的链表的语句是（  ）
```

- [ ] `a.next=c; c.next=b;`
- [ ] `p.next=q;q.next=p.next;`
- [x] `q->next=&b;p->next=q;`
- [ ] `p->next=&c;q->next=p->next;`

当定义一个结构体变量时，系统分配给它的内存是（ ）。

- [x] `各成员所需内存量的总和`
- [ ] `成员中占内存量最大的容量`
- [ ] `结构体中第一个成员所需内存量`
- [ ] `结构体中最后一个成员所需内存量`

以下对结构体类型变量的定义中不正确的是(  )。

- [ ] ```c
  struct {
  int num;
  float age;
  } std1 ;
  ```

- [ ] ```c
  #define STUDENT struct student 
     STUDENT { 
  int num ; float age ;
  } std1 ;
  ```

- [ ] ```c
  struct student {
  int num ;
  float age ;
  }std1 ;
  ```

- [x] ```c
  struct {
  int num ; float age ;
  } student ;
  struct student std1 ;
  
  ```

```c
以下对结构体变量成员不正确的引用是(   )。
struct pupil {
   char name[20]; int age; int sex ;
} pup[5], *p=pup ; 
```

- [ ] `scanf("%d",&pup[0].age);`
- [ ] `scanf("%s",pup[0].name);`
- [x] `scanf("%d",p->age);`
- [ ] `scanf("%d",&(p->sex));`









### 9

系统的标准输入设备是指（  ）。

- [ ] `硬盘`
- [x] `键盘`
- [ ] `软盘`
- [ ] `显示器`

若以”a+”方式打开一个已存在的文件，则以下叙述正确的是（  ）。

- [ ] `文件打开时，原有文件内容被删除，只可作写操作`

- [x] `文件打开时，原有文件内容不被删除，位置指针移到文件末尾，可作添加和读操作`

- [ ] `文件打开时，原有文件内容不被删除，位置指针移到文件开头，可作重写和读操作`

- [ ] `以上说法都不正确`

函数rewind的作用是（  ）。

- [ ] `使位置指针指向文件的末尾`
- [x] `使位置指针重新返回文件的开头`
- [ ] `将位置指针指向文件中所要求的特定位置`

- [ ] `使位置指针自动移至下一个字符位置`

若要用fopen函数打开一个新的二进制文件，该文件既要能读也能写，则文件打开方式字符串应是（ ）。

- [x] `"wb+"`
- [ ] `"ab"`
- [ ] `"ab+"`
- [ ] `"rb+"`

函数ftell(fp)的作用是（  ）。

- [x] `得到流式文件中的当前位置`

- [ ] `初始化流式文件的位置`

- [ ] `以上答案均正确`
- [ ] `移动流式文件的位置指针`

fgetc函数的作用是从指定文件读入一个字符，该文件的打开方式必须是（ ）。

- [ ] `只写`

- [x] `追加、读或读写`

- [ ] `读或读写`
- [ ] `追加`

利用fseek函数可实现的操作是（  ）。

- [x] `改变文件的位置指针`
- [ ] `从磁盘里读写`

- [ ] `文件的随机读写`

- [ ] `文件的顺序读写`

若执行fopen函数时发生错误，则函数的返回值是（ ）。

- [ ] `EOF`

- [ ] `1`
- [ ] `地址值`
- [x] `0`

函数调用语句：fseek(fp,-20L,2)的含义是（  ）。

- [ ] `将文件位置指针移到当前位置20个字节处`

- [ ] `将文件位置指针从当前位置向后移动20个字节`
- [ ] `将文件位置指针移到距离文件头20个字节处`
- [x] `将文件位置指针从文件末尾向后退20个字节`

能作为输入文件名字符串常量的是指（ ）。

- [ ] `c:user\text.txt`

- [ ] `c:\user\text.txt`

- [x] `"c:\\user\\text.txt"`

- [ ] `"c:\user\text.txt"`





## 程序设计

### 6

#### 6.1

```c
/*请编写函数fun,其功能是:将两个两位数的正整数a、b合并形成一个整数放在c中。
合并的方式是:将a数的十位和个位依次放在c数的千位和十位上,b数的十位和个位依次放在c数的百位和个位上。
例如,当a=45,b=12,调用该项函数后,c=4152。 
注意:部分源程序给出如下。 
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。
试题程序: */
#include <stdio.h>
#include <conio.h>
void fun(int a ,int b,long *c)
{
  /************Begin************/



  /************End***************/
}
int main()
{
  int  a,b,i;  
  long c;
  FILE *out,*in;
  printf("Input a ,b: ");
  scanf("%d%d",&a,&b);
  fun(a,b,&c);
  printf("The result is :%ld\n",c);
  /******************************/
  in=fopen("in20.dat","r");
  out=fopen("out20.dat","w");
  for(i=10;i<20;i++)
  {
   fscanf(in,"%d %d",&a,&b);
	fun(a,b,&c);
	fprintf(out,"%d\n",c);
  }
fclose(out);
fclose(in);
/******************************/
return 0;
}

```



```c
/*?????fun,????:??????????a?b??????????c??
??????:?a???????????c????????,b???????????c?????????
??,?a=45,b=12,???????,c=4152? 
??:?????????? 
????main?????????????,????fun????????????????
????: */
#include <stdio.h>
//#include <conio.h>
void fun(int a ,int b,long *c)
{
  /************Begin************/
    *c=(a/10)*1000+(b/10)*100+(a%10)*10+(b%10);


  /************End***************/
}
int main()
{
  int  a,b,i;  
  long c;
  FILE *out,*in;
  printf("Input a ,b: ");
  scanf("%d%d",&a,&b);
  fun(a,b,&c);
  printf("The result is :%ld\n",c);
  /******************************/
  in=fopen("in20.dat","r");
  out=fopen("out20.dat","w");
  for(i=10;i<20;i++)
  {
   fscanf(in,"%d %d",&a,&b);
	fun(a,b,&c);
	fprintf(out,"%d\n",c);
  }
fclose(out);
fclose(in);
/******************************/
return 0;
}

```

看了这题的out.dat，有被年份感动到。



#### 6.2

```c
/*请编一个函数fun(char *s),该函数的功能是把字符串中的内容逆置。
例如,字符串中原有的字符串为abcdefg,则调用该函数后,串中的内容为gfedcba。
注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。
试题程序:*/
#include <string.h>
#include <stdio.h>
#define N 81
void fun(char*s)
{
/************Begin*************/


/************End**************/
}
int main()
{
	 char a[N];
	 FILE *out,*in;
	 printf("Enter a string:");
	 gets(a);
	 printf("The  original string is:");
	 puts(a);
	 fun(a);
	 printf("\n");
	 printf("The string after modified:");
	 puts(a);
	 strcpy(a,"Hello World! This is a first C program!");
	 fun(a);
	 /******************************/
      in=fopen("in17.dat","r");
      fgets(a,81,in);
	 out=fopen("out17.dat","w");
        fun(a);
	 fprintf(out,"%s",a);
	 fclose(out);
       fclose(in);
	 /******************************/
      return 0;
}

```



```c
/*??????fun(char *s),??????????????????
??,???????????abcdefg,???????,??????gfedcba?
??:??????????
????main?????????????,????fun????????????????
????:*/
#include <string.h>
#include <stdio.h>
#define N 81
void fun(char*s)
{
/************Begin*************/
    int t,i=0,j,n=0;
    while (s[n]) {n++;}
    for (i=0,j=n-1;i<=j;i++,j--) {
        t=s[i];
        s[i]=s[j];
        s[j]=t;
    }
/************End**************/
}
int main()
{
	 char a[N];
	 FILE *out,*in;
	 printf("Enter a string:");
	 gets(a);
	 printf("The  original string is:");
	 puts(a);
	 fun(a);
	 printf("\n");
	 printf("The string after modified:");
	 puts(a);
	 strcpy(a,"Hello World! This is a first C program!");
	 fun(a);
	 /******************************/
      in=fopen("in17.dat","r");
      fgets(a,81,in);
	 out=fopen("out17.dat","w");
        fun(a);
	 fprintf(out,"%s",a);
	 fclose(out);
       fclose(in);
	 /******************************/
      return 0;
}

```







#### 6.3

```c
/*请编写函数fun,该函数的功能是:判断字符串是否为回文,若是则函数返回1,主函数中输出"YES",否则返回0,主函数中输出"NO"。
回文是指顺读和倒读都一样的字符串。例如,字符串LEVEL是回文,而字符串123312就不是回文。
注意:部分源程序给出如下。请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。
试题程序:*/
#include <stdio.h>
#define N 80
int fun(char str[])
{
    /***************Begin************/


    /*************** End ************/
}
int main()
{
	 char s[N];
	 FILE *out,*in;
         char test[][80]={"1234321","123421","123321","abcdCBA"};
	 int i;
	 printf("Enter a string : ");
	 gets(s);
	 printf("\n\n");
	 puts(s);
	 if(fun(s))
		printf("YES\n");
	 else
		printf("NO\n"); 
	 /************************************/
    in=fopen("in12.dat","r");
    for(i=0;i<4;i++)
    fscanf(in,"%s",test[i]);
	 out=fopen("out12.dat","w");
	 for(i=0;i<4;i++)
	 	if(fun(test[i]))
			fprintf(out,"YES\n");
		else
			fprintf(out,"NO\n");
    fclose(in);
	 fclose(out);
	 /************************************/
  return 0;
}

```



```c
/*?????fun,???????:??????????,???????1,??????"YES",????0,??????"NO"?
???????????????????,???LEVEL???,????123312??????
??:??????????????main?????????????,????fun????????????????
????:*/
#include <stdio.h>
#define N 80
int fun(char str[])
{
    /***************Begin************/
    int i,j,n=0,ju=1;
    while (str[n]) {n++;}
    for (i=0,j=n-1;i<j;i++,j--) {
        if (str[i]!=str[j]) {
            ju=0;
            break;
        }
    }
    return ju;

    /*************** End ************/
}
int main()
{
	 char s[N];
	 FILE *out,*in;
         char test[][80]={"1234321","123421","123321","abcdCBA"};
	 int i;
	 printf("Enter a string : ");
	 gets(s);
	 printf("\n\n");
	 puts(s);
	 if(fun(s))
		printf("YES\n");
	 else
		printf("NO\n"); 
	 /************************************/
    in=fopen("in12.dat","r");
    for(i=0;i<4;i++)
    fscanf(in,"%s",test[i]);
	 out=fopen("out12.dat","w");
	 for(i=0;i<4;i++)
	 	if(fun(test[i]))
			fprintf(out,"YES\n");
		else
			fprintf(out,"NO\n");
    fclose(in);
	 fclose(out);
	 /************************************/
  return 0;
}

```





#### 6.4

```c
/*请编写函数fun,该函数的功能是:统计一行字符串中单词的个数,作为函数值返回。
一行字符串在主函数中输入,规定所有单词由小写字母组成,单词之间有若干个空格隔开,一行的开始没有空格。 
注意:部分源程序给出如下。 
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。 
试题程序:*/
#include<string.h>
#include<stdio.h>
#define N 80
int fun(char *s)
{
 /************Begin*************/



/*************End*************/
}
int main()
{ 
  FILE *wf,*in;
  char line[N]; 
  int num=0;
  printf("Enter a string:\n "); 
  gets(line);
  num=fun(line);
  printf("The number of word is:%d\n\n ",num);
/******************************/
 in=fopen("in19.dat","r");
  wf=fopen("out19.dat","w");
  fgets(line,81,in);
  fprintf(wf,"%d",fun(line));
  fclose(wf);
  fclose(in);
/*****************************/
  return 0;
}
```

Pointer:

```c
/*?????fun,???????:?????????????,????????
????????????,?????????????,????????????,?????????? 
??:?????????? 
????main?????????????,????fun???????????????? 
????:*/
#include<string.h>
#include<stdio.h>
#define N 80
int fun(char *s)
{
 /************Begin*************/
    int i=0,num=0;
    while (*s!=0) {
        if (*s>='a'&& *s<='z') {
            if (*(s+1)<'a'||*(s+1)>'z') {
                num++;
            }
        }
        s++;
    }
    return num;
/*************End*************/
}
int main()
{ 
  FILE *wf,*in;
  char line[N];
  int num=0;
  printf("Enter a string:\n ");
  gets(line);
  num=fun(line);
  printf("The number of word is:%d\n\n ",num);
/******************************/
 in=fopen("in19.dat","r");
  wf=fopen("out19.dat","w");
  fgets(line,81,in);
  fprintf(wf,"%d",fun(line));
  fclose(wf);
  fclose(in);
/*****************************/
  return 0;
}
```

Array:

```c
/*?????fun,???????:?????????????,????????
????????????,?????????????,????????????,?????????? 
??:?????????? 
????main?????????????,????fun???????????????? 
????:*/
#include<string.h>
#include<stdio.h>
#define N 80
int fun(char *s)
{
 /************Begin*************/
    int i=0,num=0;
    while (s[i]!=0) {
        if (s[i]>='a'&& s[i]<='z') {
            if (s[i+1]<'a'||s[i+1]>'z') {
                num++;
            }
        }
        i++;
    }
    return num;
/*************End*************/
}
int main()
{ 
  FILE *wf,*in;
  char line[N];
  int num=0;
  printf("Enter a string:\n ");
  gets(line);
  num=fun(line);
  printf("The number of word is:%d\n\n ",num);
/******************************/
 in=fopen("in19.dat","r");
  wf=fopen("out19.dat","w");
  fgets(line,81,in);
  fprintf(wf,"%d",fun(line));
  fclose(wf);
  fclose(in);
/*****************************/
  return 0;
}
```





#### 6.5

```c
/*假定输入的字符串中只包含字母和*号。请编写函数fun,它的功能是:将字符串中的前导*号全部删除,中间和后面的*号不删除。
例如,若字符串中的内容为****A*BC*DEF*G*******,删除后,字符串中的内容则应当是A*BC*DEF*G*******。
注意:部分源程序给出如下。 
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。 
试题程序: */
#include <stdio.h>
void  fun  (char *a)
{
/************Begin**************/



/************End*************/
}
int main()
{
  FILE *wf,*in;
  int i;
  char s[81],t[81]="****A*BC*DEF*G*******";
  printf("Enter a string :\n");
  gets(s);
  fun(s);
  printf("The string after deleted:\n");puts(s);
/******************************/
  in=fopen("in18.dat","r");
  wf=fopen("out18.dat","w");
  for(i=0;i<8;i++)
  {
	  fscanf(in,"%s",t);
	  fun(t);
      fprintf(wf,"%s\n",t);
  }
  fclose(in);
  fclose(wf);
/*****************************/
 return 0;
}
```

这种做法似乎会使得输出为空，难道是另字符数组元素为0会自动使字符串“失效”嘛？是不是计算机太着急了？

```c
  int n=0,i;
  while (*(a+n)=='*') {
    *(a+n)=0;
    n++;
  }
  while (*(a+n+i)) {
    *(a+i)=*(a+n+i);
    *(a+n+i)=0;
    i++;
  }
```

后来发现是因为忘记初始化i了，😄

```c
/*???????????????*???????fun,?????:????????*?????,??????*?????
??,?????????****A*BC*DEF*G*******,???,???????????A*BC*DEF*G*******?
??:?????????? 
????main?????????????,????fun???????????????? 
????: */
#include <stdio.h>
void  fun  (char *a)
{
/************Begin**************/
    int n=0,i=0;
    while (*(a+n)=='*') {
        *(a+n)=0;
        n++;
    }
    while (*(a+n+i)) {
        *(a+i)=*(a+n+i);
        *(a+n+i)=0;
        i++;
    }
/************End*************/
}
int main()
{
  FILE *wf,*in;
  int i;
  char s[81],t[81]="****A*BC*DEF*G*******";
  printf("Enter a string :\n");
  gets(s);
  fun(s);
  printf("The string after deleted:\n");puts(s);
/******************************/
  in=fopen("in18.dat","r");
  wf=fopen("out18.dat","w");
  for(i=0;i<8;i++)
  {
	  fscanf(in,"%s",t);
	  fun(t);
      fprintf(wf,"%s\n",t);
  }
  fclose(in);
  fclose(wf);
/*****************************/
 return 0;
}
```





#### 6.6

```c
/*假定输入的字符串中只包含字母和*号。请编写函数fun,它的功能是:除了字符串前导的*号之外,将串中其他*号全部删除。
在编写函数时,不得使用C语言提供的字符串函数。 
例如,若字符串中的内容为****A*BC*DEF*G*******,删除后,字符串中的内容则应当是****ABCDEFG。 
注意:部分源程序给出如下。 
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。 
试题程序: */
#include <string.h>
#include <stdio.h>
void  fun  (char *a)
{
/************Begin*************/



/************End**************/
}
int main()
{
  char s[81];
  FILE *in,*out;
  int i;
  printf("Enter a string :\n");
  gets(s);
  fun(s);
  printf("The string after deleted:\n");
  puts(s);
  /******************************/
  in=fopen("in21.dat","r");
  out=fopen("out21.dat","w");
  for(i=0;i<8;i++)
  {
	  fscanf(in,"%s",s);
	  fun(s);
      fprintf(out,"%s\n",s);
  }
  fclose(in);
  fclose(out);
  /******************************/
  return 0;
}

```



```c
/*???????????????*???????fun,?????:????????*???,?????*??????
??????,????C??????????? 
??,?????????****A*BC*DEF*G*******,???,???????????****ABCDEFG? 
??:?????????? 
????main?????????????,????fun???????????????? 
????: */
#include <string.h>
#include <stdio.h>
void  fun  (char *a)
{
/************Begin*************/
    int i=0,j,x,k;
    while (a[i]=='*') {
        if (a[++i]!='*') break;
    }
    x=i-1;
    while (a[i]) {
        if (a[i]=='*') {
            a[i]=0;
        }
        i++;
    }
    for (j=i-1;j>x;j--) {
        if (a[j]==0) {
            for (k=j;k<i;k++) {
                a[k]=a[k+1];
            }
        }
    }

/************End**************/
}
int main()
{
  char s[81];
  FILE *in,*out;
  int i;
  printf("Enter a string :\n");
  gets(s);
  fun(s);
  printf("The string after deleted:\n");
  puts(s);
  /******************************/
  in=fopen("in21.dat","r");
  out=fopen("out21.dat","w");
  for(i=0;i<8;i++)
  {
	  fscanf(in,"%s",s);
	  fun(s);
      fprintf(out,"%s\n",s);
  }
  fclose(in);
  fclose(out);
  /******************************/
  return 0;
}

```

### 8

#### 8.1

```c
/*有n个学生，每个学生的数据包括学号，C语言程序设计课程的平时成绩和期末考试成绩，，测试数据已在主函数中，实现按平时成绩占30%，期末成绩占70%计算总评成绩，
将总评成绩平均分以上的学生的等级确定为"均分以上"，同时将这些同学的对应信息存放在结构体数组h中，人数通过函数返回值得到。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中注释语句之间填入所编写的若干语句。*/
#include <stdio.h>
#include<string.h>
#include<stdlib.h>
#define  N 100
typedef  struct
{ char num[10];/*学号*/
  int s1;/*期末成绩*/
  int s2;/*平时成绩*/
  float sum; /*总评*/
  char level[10]; /*等级*/
} STU;
int fun (STU a[],int n,STU h[])
{
/************Begin************/


```





#### 8.2

```c
/*学生的记录由学号和成绩组成，N名学生的数据已在主函数中放入结构体数组s中,请编写函数fun，它的功能是：
把分数最高的学生数据放在b所指的数组中,注意：分数最高的学生可能不止一个，函数返回分数最高的学生的人数。 
注意: 部分源程序在如下。 
请勿改动主函数main和其它函数中的任何内容，仅在函数fun的花括号中填入 
你编写的若干语句。 
给定源程序： */
#include <stdio.h> 
#define N 16 
typedef struct 
{	 char num[10]; 
int s; 
} STREC; 
int fun( STREC *a, STREC *b ) 
{
   /**************Begin*************/




   /*************End***************/
    
} 
int main() 
{ STREC s[N]={{"GA05",85},{"GA03",76},{"GA02",69},{"GA04",85}, 
  {"GA01",91},{"GA07",72},{"GA08",64},{"GA06",87}, 
  {"GA015",85},{"GA013",91},{"GA012",64},{"GA014",91}, 
  {"GA011",77},{"GA017",64},{"GA018",64},{"GA016",72}}; 
STREC h[N]; 
   int i,n;
   FILE *out,*in;
   n=fun(s,h);
   printf("The %d highest score :\n",n);
   for(i=0;i<n; i++)
     printf("%s  %4d\n",h[i].num,h[i].s);
   printf("\n");
   out = fopen("out03.dat","w");
   in=fopen("in03.dat","r");
   i=0;
   while(!feof(in))
   {
      fscanf(in,"%s %d\n",h[i].num,&h[i].s);
      i++;
   }
   n=fun(s,h);
   for(i=0;i<n; i++)
   {
     fprintf(out, "%s %d\n",h[i].num,h[i].s);
   }
   fclose(in);
   fclose(out);
return 0;
} 

```







#### 8.3

```c
/*有n个学生，每个学生的数据包括学号，C语言程序设计课程的平时成绩和期末考试成绩，测试数据已在主函数中，要求按平时成绩占30%，期末成绩占70%计算总评成绩，
并将总评成绩低于90分，且高于等于80分的同学的等级确定为"良好"，并将这些同学的对应信息存放在结构体数组h中，人数通过函数返回值得到，输出相应的信息。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中注释语句之间填入所编写的若干语句。*/
#include <stdio.h>
#include<string.h>
#include<stdlib.h>
#define  N 100
typedef  struct
{ char num[10];/*学号*/
  int s1;/*期末成绩*/
  int s2;/*平时成绩*/
  float sum; /*总评*/
  char level[10]; /*等级*/
} STU;
int fun (STU a[],int n,STU h[])
{
/************Begin************/
  




 /************End**************/
}
int main()
{
  STU s[N]={{"GA05",85,76},{"GA03",76,90},{"GA02",69,90},{"GA04",85,56},{"GA01",91,95},
				{"GA07",72,80},{"GA08",64,45},  {"GA06",87,98},{"GA015",85,86},{"GA013",91,97}},h[N];
  int i,k,n=10; 
  FILE *out,*in;
  k=fun(s,n,h);
  printf("There are :\n");
  for(i=0;i<k;i++)
    printf("%s %d %d %.2f %s\n",h[i].num,h[i].s1,h[i].s2,h[i].sum,h[i].level);
  /******************************/
  in=fopen("in68.dat","r");
  out=fopen("out68.dat","w");
  i=0;
  while(!feof(in))
  {
  	fscanf(in,"%s %d %d",s[i].num,&s[i].s1,&s[i].s2);
  	i++;
  }
  n=i;
  k=fun(s,n,h);
  for(i=0;i<k;i++)
    fprintf(out,"%s %d %d %.2f %s\n",h[i].num,h[i].s1,h[i].s2,h[i].sum,h[i].level);
  fclose(out);
  fclose(in);
  /******************************/
  system("pause");
  return 0;
}

```







#### 8.4

```c
/*学生的记录由学号和成绩组成,N名学生的数据已在主函数中放入结构体数组s中,请编写函数fun,
它的功能是:把指定分数范围内的学生数据放在b所指的数组中,分数范围内的学生人数由函数值返回。
例如,输入的分数是60和69,则应当把分数在60到69的学生数据进行输出,包含60分和69分的学生数据。
主函数中把60放在low中,把69放在heigh中。注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。
试题程序: */
#include <stdio.h>
#define  N  16
typedef  struct
{ char num[10];
  int  s ;
}STREC;
int  fun (STREC *a, STREC *b, int l, int h )
{
/************Begin*************/




/************End************/
}

int main ()
{
  FILE *wf,*in;
  STREC  s[N]={{ "GA005",85},{"GA003",76},{"GA002",69},{"GA004",85},
  {"GA001",96},{"GA007",72},{"GA008",64},{"GA006",87},
  {"GA015",85},{"GA013",94},{"GA012",64},{"GA014",91},
  {"GA011",90},{"GA017",64},{"GA018",64},{"GA016",72}};
  STREC h[N],tt; 
  int i, j,n, low, heigh, t;
  printf("Enter 2 integer number low & heigh: ");
  scanf("%d%d",&low,&heigh);
  if(heigh<low) 
    {t=heigh;heigh=low; low=t;}
  n=fun(s,h,low, heigh);
  printf("The student 's data between %d--%d:\n ",low, heigh);
  for(i=0;i<n;i++)
     printf("%s %4d\n ",h[i].num, h[i].s);    /*输出指定分数范围内的学生记录*/
  printf("\n ");
/******************************/
 in=fopen("in26.dat","r");
 i=0;
 while(!feof(in))
 {
     fscanf(in,"%s %d\n",s[i].num,&s[i].s);
     i++;
  }
  n=fun(s,h,80,98);
  for(i=0;i<n-1;i++)          /*分数在80～98之间的学生记录按分数从低到高排列*/
     for(j=i+1;j<n;j++)
        if(h[i].s>h[j].s) 
          {tt=h[i];h[i]=h[j];h[j]=tt;}
  wf=fopen("out26.dat","w");
  for(i=0;i<n;i++)
     fprintf(wf, "%s %4d\n",h[i].num, h[i].s);
  fclose(in);
  fclose(wf);
/*****************************/
return 0;
}

```





#### 8.5

```c
/*有n个学生，每个学生的数据包括学号，C语言程序设计课程的平时成绩和期末考试成绩，测试数据已在主函数中，要求按平时成绩占30%，期末成绩占70%计算总评成绩，
并将总评成绩低于60分的同学的等级确定为"不及格"，其余同学为"及格"，并输出相应的信息。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中注释语句之间填入所编写的若干语句。*/
#include <stdio.h>
#include<string.h>
#include<stdlib.h>
#define  N 100
typedef  struct
{ char num[10];/*学号*/
  int s1;/*期末成绩*/
  int s2;/*平时成绩*/
  float sum; /*总评*/
  char level[10]; /*等级*/
} STU;
void fun (STU a[],int n)
{
/************Begin************/
  
 



 /************End**************/
}
int main()
{
  STU s[N]={{"GA05",85,76},{"GA03",76,90},{"GA02",69,90},{"GA04",85,56},{"GA01",91,95},
				{"GA07",72,80},{"GA08",64,45},  {"GA06",87,98},{"GA015",85,86},{"GA013",91,97}};
  int i,n=10; 
  FILE *out,*in;
  fun(s,n);
  printf("There are :\n");
  for(i=0;i<n;i++)
    printf("%s %d %d %.2f %s\n",s[i].num,s[i].s1,s[i].s2,s[i].sum,s[i].level);
  /******************************/
  in=fopen("in67.dat","r");
  out=fopen("out67.dat","w");
  i=0;
  while(!feof(in))
  {
  	fscanf(in,"%s %d %d",s[i].num,&s[i].s1,&s[i].s2);
  	i++;
  }
  n=i;
  fun(s,n);
  for(i=0;i<n;i++)
    fprintf(out,"%s %d %d %.2f %s\n",s[i].num,s[i].s1,s[i].s2,s[i].sum,s[i].level);
  fclose(out);
  fclose(in);
  /******************************/
  system("pause");
  return 0;
}

```





#### 8.6

```c
/*学生的记录由学生姓名、学号、语文、数学、英语三门成绩组成,N名学生的数据已在主函数中放入结构体数组s中,
请编写函数fun,其功能是:把三门总分最低的学生数据放在h所指的数组中。注意:分数最低的学生可能不止一个,
函数返回分数最低的学生的人数。 注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的花括号中填入所编写的若干语句。试题程序:*/
#include <stdio.h>
# define  N 6
typedef  struct
{ 
	char name[10];
	long num;
	int s1;
	int s2;
	int s3;
	int s;
} STREC;
int fun (STREC *a,STREC *b,int m)
{
  /***********Begin*************/






  /**********End***************/
}
int main()
{
  STREC s[100]={{"GA01",1,80,56,87},{"GA03",3,76,56,54},{"GA02",2,69,63,54},{"GA04",4,85,98,90},{"GA05",5,91,94,95},{"GA06",6,72,80,87}};
  STREC h[100]; 
  int i,n,m;  
  FILE *out,*in;
  n=fun(s,h,N);
  printf("The %d lowest score:\n",n);
  for(i=0;i<n;i++)
    printf("%s %4d\n",h[i].name,h[i].s);
  printf("\n");
  /******************************/
  in=fopen("in53.dat","r");
  out=fopen("out53.dat","w");
  fscanf(in,"%d\n",&m);
  for(i=0;i<m;i++)
    fscanf(in,"%s %ld %d %d %d\n",s[i].name,&s[i].num,&s[i].s1,&s[i].s2,&s[i].s3);
  n=fun(s,h,m);
  fprintf(out,"%d\n",n);
  for(i=0;i<n;i++)
  	fprintf(out,"%s %d\n",h[i].name,h[i].s);
  fclose(in);
  fclose(out);
  /******************************/
  return 0;
}

```







## 程序改错

### 6

#### 6.1

```c
/*假定输入的字符串中只包含字母和*号。函数fun的功能是:将字符串中的前导*号全部删除,中间和后面的*号不删除。
例如,若字符串中的内容为****A*BC*DEF*G*******,删除后,字符串中的内容则应当是A*BC*DEF*G*******。
注意:不得增行或删行,也不得更改程序的结构。
试题程序:
*/
#include <stdio.h>
#include<stdlib.h>
/**********ERROR**********/
void  fun(char *a);
{
    char *p=a;
/**********ERROR**********/
     while(*p!='*')
        p++; 
/**********ERROR**********/
    for(;*p!='\0';p++)
        *a=*p;
/**********ERROR**********/
    *a="\0"; 
}
int main()
{
	char s[81];
	printf("Enter a string :\n");
	gets(s);
/**********ERROR**********/
	fun(&s[80]);
	printf("The string after deleted:\n");
	puts(s);
       system("pause");
	return 0;
}

```

```c
【改错1】	错误
【学生答案】
void  fun(char *a);
【参考答案】
void  fun(char *a)
void  fun(char a[])

==============================
【改错2】	错误
【学生答案】
while(*p!='*')
【参考答案】
while(*p=='*')
*p=='*'
'*'==*p

==============================
【改错3】	错误
【学生答案】
for(;*p!='\0';p++)
【参考答案】
for(;*p!='\0';p++,a++)
for(;*p!='\0';a++,p++)
a++,p++
p++,a++
++a,++p
++p,++a
a=a+1,p++
p++,a=a+1
p++,a+=1
a+=1,p++

==============================
【改错4】	错误
【学生答案】
*a="\0"; 
【参考答案】
*a=0;
*a='\0';

==============================
【改错5】	错误
【学生答案】
fun(&s[80]);
【参考答案】
fun(s);
fun(&s[0]);

==============================

```

比我在程序设计里写得好。



#### 6.2

```c
/*下列给定程序中,函数fun的功能是:计算s所指字符串中含有t所指字符串的数目,并作为函数值返回。 
请改正函数fun中的错误或在横线处填上适当的内容并把横线删除,使它能得出正确的结果。
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。
试题程序:*/
#include  <stdlib.h>
#include  <string.h>
#include  <stdio.h>
#define N 80
int fun(char *s,char *t)
{ int n;
  char *p, *r;
  n=0;
  p=&s[0];
/**********ERROR**********/
  *r=t;
  while(*p)
  { 
	if(*r==*p)
	{
		r++;
		if(*r=='\0')
		{	
			n++;
/**********ERROR**********/
			t=r;
		}
	}
  	p++;
  }
  return n;
}
int main()
{char a[N],b[N]; int m;
printf("\nPlease enter string a: ");
gets(a);
 printf("\nPlease enter substring b: ");
gets(b);
/**********ERROR**********/
 m=fun(a[N],b[N]);
 m=printf("\nThe result is :m=%d\n",m);
return 0;
}

```



```c
【改错1】	错误
【学生答案】
*r=t;
【参考答案】
r=t;

==============================
【改错2】	错误
【学生答案】
t=r;
【参考答案】
r=t;
r=&t[0];

==============================
【改错3】	错误
【学生答案】
m=fun(a[N],b[N]);
【参考答案】
m=fun(a,b);

==============================

```



#### 6.3

```c
/*下列给定程序中函数fun的功能是:先将在字符串s中的字符按逆序存放到t串中,然后把s中的字符按正序连接到t串的后面。
例如,当s中的字符串为ABCDE时,则t中的字符串应为EDCBAABCDE。
请改正程序中的错误,使它能得出正确的结果。
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。
试题程序: */
#include  <stdlib.h>
#include  <stdio.h>
#include  <string.h>
void fun (char *s, char *t )
{
  int i,s1;
  s1=strlen(s);    
  for (i=0;i<s1;i++)
/**********ERROR**********/
      t[i]=s[s1-1];    
  for (i=0;i<s1;i++)
      t[s1+i]=s[i];
/**********ERROR**********/
  t[2*s1]='0';
}
int main()
{char s[100], t[100];
  printf("\nPlease enter string s: "); 
  scanf("%s",s);
/**********ERROR**********/
  fun(s[100],t[100]);
  printf ("The result is: %s\n",t);
return 0;
}

```



```c
【改错1】	错误
【学生答案】
t[i]=s[s1-1];    
【参考答案】
t[i]=s[s1-1-i];
t[i]=s[s1-i-1];

==============================
【改错2】	错误
【学生答案】
t[2*s1]='0';
【参考答案】
t[2*s1]='\0';
t[2*s1]=0;

==============================
【改错3】	错误
【学生答案】
fun(s[100],t[100]);
【参考答案】
fun(s,t);

==============================

```



#### 6.4

```c
/*下列给定程序中函数fun的功能是:将长整型数中每一位上为奇数的数依次取出,构成一个新数放在t中。高位仍在高位,低位仍在低位。
例如当s中的数为87653142时,t中的数为7531。 请改正函数fun中的错误,使它能得出正确的结果。 
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。  试题程序:*/
#include  <stdlib.h>
#include  <stdio.h>
void fun(long s,long *t)
{int d;
 long s1=1;
/**********ERROR**********/
 t=0;
 while(s>0)
    { d=s%10;
/**********ERROR**********/
      if(d%2==0)
        {*t=d*s1+*t;
         s1*=10;
        }
    s/=10;
    }
}  
int main()
{
long s, t;
printf("\nPlease enter s: "); scanf("%ld",&s);
/**********ERROR**********/
 fun(s,t);
 printf("The result is :%ld\n",t);
return 0;
}

```



```c
【改错1】	错误
【学生答案】
t=0;
【参考答案】
*t
*t=0;

==============================
【改错2】	错误
【学生答案】
if(d%2==0)
【参考答案】
if(d%2!=0)
if(d%2)
if(d%2==1)

==============================
【改错3】	错误
【学生答案】
fun(s,t);
【参考答案】
fun(s,&t);

==============================

```



#### 6.5

```c
/*下列给定程序中,函数fun的功能是:在字符串str中找出ASCII码值最大的字符,将其放在第一个位置上,
并将该字符前的原字符向后顺序移动。例如,调用fun函数之前给字符串输入ABCDeFGH,调用后字符串中的内容为eABCDFGH。
请改正程序中的错误,使它能得出正确的结果。
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。
试题程序: */
#include <stdio.h>
/**********ERROR**********/
fun(char *p)
{ char max, *q;int i=0;
  max=p[i];
  while (p[i]!=0)
       {if (max<=p[i])
          { 
/**********ERROR**********/
           p = q +i;max=p[i];
          }
        i++;
       }
/**********ERROR**********/
  while(q<p)
      {*q=*(q-1);
        q--;
       }
  p[0]=max;
}
int main()
{char str[80];
  printf("Enter a string: "); gets(str);
  printf("\nThe original string: "); 
puts(str);
  fun(str);
  printf("\nThe string after moving: ");
puts(str); printf("\n\n");
return 0;
}

```



```c
【改错1】	错误
【学生答案】
fun(char *p)
【参考答案】
void fun(char *p)

==============================
【改错2】	错误
【学生答案】
p = q +i;max=p[i];
【参考答案】
q=p+i;
q=i+p;

==============================
【改错3】	错误
【学生答案】
while(q<p)
【参考答案】
while(q>p)
while(p<q)

==============================

```



#### 6.6

```c
/*下列给定程序中,函数fun的功能是:在字符串str中找出ASCII码值最大的字符,将其放在第一个位置上,并将该字符前的原字符向后顺序移动。
例如,调用fun函数之前给字符串输入ABCDeFGH,调用后字符串中的内容为eABCDFGH。 
请改正程序中的错误,使它能得出正确的结果。 
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。 
试题程序: */
#include <stdio.h>
/**********ERROR**********/
int fun(char *p)
{ 
char max, *q;
int i=0;
  max=p[i];
  while (p[i]!=0)
       {if (max<=p[i])
          { 
/**********ERROR**********/
           p = q +i;
max=p[i];
          }
        i++;
       }
/**********ERROR**********/
  while(q<p)
      {*q=*(q-1);
        q--;
       }
  p[0]=max;
}
int main()
{
char str[80];
  printf("Enter a string: "); 
gets(str);
  printf("\nThe original string: "); 
puts(str);
  fun(str);
  printf("\nThe string after moving: ");
puts(str); 
printf("\n\n");
return 0;
}

```



```c
【改错1】	错误
【学生答案】
int fun(char *p)
【参考答案】
void fun(char *p)

==============================
【改错2】	错误
【学生答案】
p = q +i;
【参考答案】
q=p+i;
q=i+p;

==============================
【改错3】	错误
【学生答案】
while(q<p)
【参考答案】
q>p
p<q

==============================

```



### 8

#### 8.1

```c
/*下列给定程序中的函数Creatlink的功能是:创建带头节点的单向链表,并为各节点数据域赋0到m-1的值。 
请改正函数Creatlink中的错误,使它能得出正确的结果。 
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。 
试题程序: */
#include <stdio.h>
#include <stdlib.h>
typedef struct aa
{ int data;
  struct aa *next;
} NODE;

NODE *Creatlink(int n, int m)
{ NODE *h=NULL,*p,*s;
  int i;
  s=(NODE *)malloc(sizeof(NODE));
  h=s;
/**********ERROR**********/
  p->next=NULL;
  for(i=1;i<n;i++)
    { s=(NODE *) malloc(sizeof(NODE));
/**********ERROR**********/
      s->data=rand()/m; 
      s->next=p->next;p->next=s;  p=p->next;
    }
  s->next=NULL;
/**********ERROR**********/
  return p;
}
void outlink(NODE *h)
{ NODE  *p;
  p=h->next;
  printf("\n The LIST :\n\n HEAD");
  while(p)
    { printf("->%d",p->data); 
      p=p->next;}
  printf("\n");
}
int main()
{ NODE *head;
  head=Creatlink(8,22);
  outlink(head);
return 0;
}

```



```c
【改错1】	错误
【学生答案】
p->next=NULL;
【参考答案】
p=s;
p=h;

==============================
【改错2】	错误
【学生答案】
s->data=rand()/m; 
【参考答案】
s->data=rand()%(m);
s->data=rand()%m;

==============================
【改错3】	错误
【学生答案】
return p;
【参考答案】
return h;
return (h);

==============================

```





#### 8.2

```c
/*下列给定程序中,函数fun的功能是:对N名学生的学习成绩,按从高到低的顺序找出前m(m<=10)名学生,
并将这些学生数据存放在一个动态分配的连续存储区中,此存储区的首地址作为函数值返回。 
请改正程序中的错误,使它能得出正确的结果。 
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。 
试题程序:*/ 
#include <stdlib.h>
#include  <string.h>
#include  <stdio.h>
#include  <malloc.h>
#define N 10
typedef struct ss
   { char num[10];
     int s;
   } STU;
STU *fun(STU a[], int m)
{ STU b[N],*t;
  int i, j,k;
/**********ERROR**********/
  *t=(STU *)calloc(m,sizeof(STU));
  for(i=0;i<N;i++) b[i]=a[i];
  for(k=0;k<m;k++)
     { for (i=j=0;i<N;i++)
          if(b[i].s>b[j].s) j=i;
/**********ERROR**********/
      t[k].num=b[j].num;
      t[k].s=b[j].s;
      b[j].s=0;
     }
return t;
}
void outresult(STU a[],FILE *pf)
{ int i;
  for(i=0;i<N;i++)
  fprintf(pf, "No=%s Mark=%d\n ",
a[i].num, a[i].s);
  fprintf(pf, "\n\n ");
}
int main()
{ STU a[N]={{ "A01 ",81},{ "A02 ",89},{ "A03 ",66},{ "A04 ",87},{ "A05 ",77},
			{ "A06 ",90},{ "A07 ",79},{ "A08 ",61},{ "A09 ",80},{ "A10 ",71}};
  STU *pOrder;
  int i, m;
  printf("*****THE RESULT*****\n");
  outresult(a,stdout);
  printf("\nGive the number of the students who have better score: ");
  scanf("%d",&m);
  while(m>10)
       { printf("\nGive the number of the students who have better score: ");
  scanf("%d",&m);
}
  pOrder=fun(a,m);
  printf("***** THE RESULT*****\n");
  printf("The top :\n");
  for(i=0;i<m;i++)
     printf("%s  %d\n",pOrder[i].num, pOrder[i].s);
  free(pOrder);
return 0;
}  

```

```c
【改错1】	错误
【学生答案】
*t=(STU *)calloc(m,sizeof(STU));
【参考答案】
t=calloc(m,sizeof(STU));
t=(STU *)calloc(m,sizeof(STU));

==============================
【改错2】	错误
【学生答案】
t[k].num=b[j].num;
【参考答案】
t[k]=b[j];
strcpy(t[k].num,b[j].num);

==============================

```





#### 8.3

```c
/*下列给定程序的功能是:建立一个带头节点的单向链表,并用随机函数为各节点数据域赋值。
函数fun的作用是求出单向链表节点(不包括头节点)数据域中的最大值,并且作为函数值返回。
请改正函数fun中的错误,使它能得出正确的结果。
注意:不要改动main函数,不得增行或删行,也不得更改程序的结构。
试题程序: */
#include <stdio.h>
#include <stdlib.h>
typedef struct aa
{ int data;
  struct aa *next;
} NODE;
int fun (NODE *h)
{ int max=-1;
  NODE *p;
/**********ERROR**********/
  p=h;
  while(p)
       { if(p->data>max)
             max=p->data;
/**********ERROR**********/
      p->next=h;
       }
  return max;
}
void outresult(int s, FILE *pf)
{ fprintf(pf, "\nThe max in link :%d\n",s);
}
NODE *creatlink(int n, int m)
{ NODE *h,*p,*s;
  int i;
  h=p=(NODE *)malloc(sizeof(NODE));
  h->data=9999;
  for(i=1;i<=n;i++)
    { s=(NODE *) malloc(sizeof(NODE));
      s->data=rand()%m; s->next=p->next;
      p->next=s;  p=p->next;
    }
  p->next=NULL;
  return h;
}
void outlink(NODE *h,FILE *pf)
{ NODE  *p;
  p=h->next;
  fprintf(pf, "\n The LIST :\n\n HEAD");
  while(p)
    { 
fprintf(pf, "->%d",p->data); 
  p=p->next;}
  fprintf(pf, "\n");
}
int main()
{ NODE *head; int m;
  head=creatlink(12,100);
  outlink(head,stdout);
  m=fun(head);
  printf("\nThe RESULT :\n"); 
  outresult(m,stdout);
return 0;
}

```

```c
【改错1】	错误
【学生答案】
p=h;
【参考答案】
p=h->next;

==============================
【改错2】	错误
【学生答案】
p->next=h;
【参考答案】
p=p->next;

==============================

```













## 程序填空

### 6

#### 6.1

```c
/*给定程序的功能是:分别统计字符串中大写字母和小写字母的个数。 
例如,给字符串ss输入:AaaaBBb123CCccccd,则输出结果应为:upper=5,lower=9。
注意:部分源程序给出如下。
请勿改动函数中的其他内容,仅在横线上填入所编写的若干表达式或语句。
试题程序: */
#include <stdlib.h>
#include <stdio.h>
void fun(char *s,int *a,int *b)
{
	 while(*s)
	 {
		if(*s>='A' && *s<='Z')
/**********FILL**********/
		   [1]    ;
		if(*s>='a' && *s<='z')
/**********FILL**********/
		【2】     ;
	 	s++;
	 }
}

int main()
{
	 char s[100];
	 int upper=0,lower=0;
	 printf("\nPlease a string: ");
	 gets(s);
	 fun(s,&upper,&lower);
/**********FILL**********/
	 printf("\n upper=%d lower=%d\n",【3】     );
return 0;
} 

```



```c
【空 1 】	错误
【学生答案】
[1]    ;
【参考答案】
(*a)++
++(*a)
*a+=1
*a=*a+1

============================================================
【空 2 】	错误
【学生答案】
?2?     ;
【参考答案】
(*b)++
++(*b)
*b+=1
*b=*b+1

============================================================
【空 3 】	错误
【学生答案】
printf("\n upper=%d lower=%d\n",?3?     );
【参考答案】
upper,lower

============================================================

```



```c
/*????????:????????????????????? 
??,????ss??:AaaaBBb123CCccccd,???????:upper=5,lower=9?
??:??????????
????????????,????????????????????
????: */
#include <stdlib.h>
#include <stdio.h>
void fun(char *s,int *a,int *b)
{
	 while(*s)
	 {
		if(*s>='A' && *s<='Z')
/**********FILL**********/
             (*a)++    ;
		if(*s>='a' && *s<='z')
/**********FILL**********/
             (*b)++     ;
	 	s++;
	 }
}

int main()
{
	 char s[100];
	 int upper=0,lower=0;
	 printf("\nPlease a string: ");
	 gets(s);
	 fun(s,&upper,&lower);
/**********FILL**********/
	 printf("\n upper=%d lower=%d\n", upper,lower   );
return 0;
}
```





#### 6.2

```c
/*请补充main函数,该函数的功能是:从键盘输入两个字符串并分别保存在字符数组str1和str2中,
用字符串str2替换字符串str1前面的所有字符。注意:str2的长度不大于str1,否则需要重新输入。
例如,如果输入str1="abced",str2="fk",则输出"fkced"。 
注意:部分源程序给出如下。 
请勿改动main函数和其他函数中的任何内容,仅在main函数的横线上填入所编写的若干表达式或语句。
试题程序:*/
#include <stdlib.h>
#include<stdio.h>
#include <string.h>
int main()
{
	 char str1[81],str2[81];
	 char *p1=str1,*p2=str2;
	 do
	 {
		printf(" Input str1 \n");
		gets(str1);
		printf(" Input str2 \n");
		gets(str2);
/**********FILL**********/
	 }while(   【1】   );
/**********FILL**********/
	 while(   【2】   )
		*p1++=*p2++;
	 printf(" Display str1 \n");
/**********FILL**********/
	 puts(   【3】   );
return 0;
} 

```



```c
【空 1 】	错误
【学生答案】
}while(   ?1?   );
【参考答案】
strlen(str1)<strlen(str2)
strlen(str2)>strlen(str1)

============================================================
【空 2 】	错误
【学生答案】
while(   ?2?   )
【参考答案】
*p2
*p2!=0

============================================================
【空 3 】	错误
【学生答案】
puts(   ?3?   );
【参考答案】
str1

============================================================

```



```c
/*???main??,???????:????????????????????str1?str2?,
????str2?????str1??????????:str2??????str1,?????????
??,????str1="abced",str2="fk",???"fkced"? 
??:?????????? 
????main?????????????,??main?????????????????????
????:*/
#include <stdlib.h>
#include<stdio.h>
#include <string.h>
int main()
{
	 char str1[81],str2[81];
	 char *p1=str1,*p2=str2;
	 do
	 {
		printf(" Input str1 \n");
		gets(str1);
		printf(" Input str2 \n");
		gets(str2);
/**********FILL**********/
	 }while(strlen(str1) < strlen(str2)   );
/**********FILL**********/
	 while(  *p2    )
		*p1++=*p2++;
	 printf(" Display str1 \n");
/**********FILL**********/
	 puts(   str1   );
return 0;
} 

```



#### 6.3

```c
/*给定程序中,函数fun的功能是:在形参s所指字符串中的每个数字字符之后插入一个*号。
例如,形参s所指的字符串为:def35adh3kjsdf7。执行结果为:def3*5*adh3*kjsdf7*。
注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的横线上填入所编写的若干表达式或语句。
试题程序:*/
#include <stdio.h>
void fun(char *s )
{
	 int i,j,n;
	 for(i=0;s[i]!='\0';i++)
/**********FILL**********/
	 if(s[i]>='0'   [1]  s[i]<='9')
	{
		n=0;
/**********FILL**********/
		while(s[i+1+n]!=  [2]  )
			n++;
		for(j=i+n+1;j>i;j--)
/**********FILL**********/
		s[j+1]=   [3]    ;
		s[j+1]='*';
			i=i+1;
		}
}
int main()
{
	char s[60]="ba3a54cd23a";
	printf("\n the original string is: %s\n",s);
	fun(s);
	printf("\nthe result is: %s\n",s);
return 0;
}

```



```c
【空 1 】	错误
【学生答案】
if(s[i]>='0'   [1]  s[i]<='9')
【参考答案】
&&

============================================================
【空 2 】	错误
【学生答案】
while(s[i+1+n]!=  [2]  )
【参考答案】
0
'\0'

============================================================
【空 3 】	错误
【学生答案】
s[j+1]=   [3]    ;
【参考答案】
s[j]
*(s+j)

============================================================

```



```c
/*?????,??fun????:???s???????????????????*??
??,??s???????:def35adh3kjsdf7??????:def3*5*adh3*kjsdf7*?
??:??????????
????main?????????????,????fun???????????????????
????:*/
#include <stdio.h>
void fun(char *s )
{
	 int i,j,n;
	 for(i=0;s[i]!='\0';i++)
/**********FILL**********/
	 if(s[i]>='0'   &&  s[i]<='9')
	{
		n=0;
/**********FILL**********/
		while(s[i+1+n]!=  0  )
			n++;
		for(j=i+n+1;j>i;j--)
/**********FILL**********/
		s[j+1]=   s[j]    ;
		s[j+1]='*';
			i=i+1;
		}
}
int main()
{
	char s[60]="ba3a54cd23a";
	printf("\n the original string is: %s\n",s);
	fun(s);
	printf("\nthe result is: %s\n",s);
return 0;
}

```





#### 6.4

```c
/*请补充函数fun,该函数的功能是:在字符串的最前端加入n个*号,形成新串,并且覆盖。注意:字符串的长度最长允许为79。
注意:部分源程序给出如下。请勿改动main函数和其他函数中的任何内容,仅在函数fun的横线上填入所编若干表达式或语句。
试题程序: */
#include  <stdlib.h>
#include  <stdio.h>
#include  <string.h>
void fun(char s[],int n)  
{
 char a[80],*p;
 int i;
/**********FILL**********/
 p=【1】;   
 for(i=0;i<n;i++)  a[i]= '*';
 do 
{
/**********FILL**********/
a[i]=【2】;
    i++;
/**********FILL**********/
 }while(【3】);
 a[i]=0;
 strcpy(s,a);
}
int main()
{
int n;char s[80];
printf("\nEnter a string: ");gets(s);
 printf("\nThe string:%s\n",s);
 printf("\nEnter n (number of*):");
 scanf("%d",&n);
 fun(s,n);
 printf("\nThe string after inster:%s\n",s);
return 0;
}

```



```c
【空 1 】	错误
【学生答案】
p=?1?;   
【参考答案】
p=s;
p=&s[0];

============================================================
【空 2 】	错误
【学生答案】
a[i]=?2?;
【参考答案】
a[i]=*p++;
a[i]=*(p++);

============================================================
【空 3 】	错误
【学生答案】
}while(?3?);
【参考答案】
*p!=0
*p!='\0'

============================================================

```



```c
/*?????fun,???????:??????????n?*?,????,???????:???????????79?
??:??????????????main?????????????,????fun?????????????????
????: */
#include  <stdlib.h>
#include  <stdio.h>
#include  <string.h>
void fun(char s[],int n)  
{
 char a[80],*p;
 int i;
/**********FILL**********/
 p=s;
 for(i=0;i<n;i++)  a[i]= '*';
 do 
{
/**********FILL**********/
a[i]=*(p++);
    i++;
/**********FILL**********/
 }while(*p!=0);
 a[i]=0;
 strcpy(s,a);
}
int main()
{
int n;char s[80];
printf("\nEnter a string: ");gets(s);
 printf("\nThe string:%s\n",s);
 printf("\nEnter n (number of*):");
 scanf("%d",&n);
 fun(s,n);
 printf("\nThe string after inster:%s\n",s);
return 0;
}

```



#### 6.5

```c
/*请补充main函数,该函数的功能是:从键盘输入若干字符放到一个字符数组中,当按回车键时结束输入,
最后输出这个字符数组中的所有字符。
注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在main函数的横线上填入所编写的若干表达式或语句。
试题程序:*/
#include <stdlib.h>
#include <stdio.h>
int main()
{
	 int i=0;
	 char s[81];
	 char *p=s;
	 printf(" Input a string \n");
	 for(i=0;i<80;i++)
	 {
		s[i]=getchar();
		if(s[i]=='\n')
/**********FILL**********/
			【1】   ;
	 }
/**********FILL**********/
	 s[i]=   【2】   ;
	 printf(" display the string \n");
	 while(*p)
/**********FILL**********/
		putchar(   【3】   );
return 0;
}

```



```c
【空 1 】	错误
【学生答案】
?1?   ;
【参考答案】
break

============================================================
【空 2 】	错误
【学生答案】
s[i]=   ?2?   ;
【参考答案】
0
'\0'

============================================================
【空 3 】	错误
【学生答案】
putchar(   ?3?   );
【参考答案】
*p++
*(p++)

============================================================

```



```c
/*???main??,???????:??????????????????,??????????,
?????????????????
??:??????????
????main?????????????,??main?????????????????????
????:*/
#include <stdlib.h>
#include <stdio.h>
int main()
{
	 int i=0;
	 char s[81];
	 char *p=s;
	 printf(" Input a string \n");
	 for(i=0;i<80;i++)
	 {
		s[i]=getchar();
		if(s[i]=='\n')
/**********FILL**********/
             break;
	 }
/**********FILL**********/
	 s[i]=   0   ;
	 printf(" display the string \n");
	 while(*p)
/**********FILL**********/
		putchar(   *(p++)   );
return 0;
}

```



### 8

#### 8.1

```c
/*给定程序中,函数fun的功能是:将形参std所指结构体数组中年龄最大者的数据作为函数值返回,并在main函数中输出。
注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的横线上填入所编写的若干表达式或语句。 
试题程序: */
#include  <stdio.h>
typedef struct
{
  char name[10];
  int age;
}STD;
STD fun(STD std[],int n)
{
  STD max;
  int i;
/**********FILL**********/
  max=【1】;
  for(i=1;i<n;i++){
/**********FILL**********/
   	if(max.age<【2】)
		max=std[i];}
  return max;
}
int main()
{ 
  STD std[5]={"aaa",17,"bbb",16,"ccc",18,"eee",15};
  STD max;
  max=fun(std,5);
  printf("\nThe result is: \n ");
/**********FILL**********/
  printf("\nName :%s,Age :%d\n",【3】,max.age);
return 0;
}

```

```c
【空 1 】	错误
【学生答案】
max=?1?;
【参考答案】
std[0]
*std

============================================================
【空 2 】	错误
【学生答案】
if(max.age<?2?)
【参考答案】
std[i].age

============================================================
【空 3 】	错误
【学生答案】
printf("\nName :%s,Age :%d\n",?3?,max.age);
【参考答案】
max.name

============================================================

```





#### 8.2

```c
/*人员的记录由编号和出生年、月、日组成,N名人员的数据已在主函数中存入结构体数组std中,且编号唯一。
函数fun的功能是:找出指定编号人员的数据,作为函数值返回,由主函数输出,若指定编号不存在,返回数据中的编号为空串。 
注意:部分源程序给出如下。 
请勿改动main函数和其他函数中的任何内容,仅在函数fun的横线上填入所编写的若干表达式或语句。 
试题程序: */
#include <stdio.h>
#include <string.h>
#define N 8
typedef struct
{
  	char num[10];
	int year,month,day;
}STU;
/**********FILL**********/
    [1]      fun(STU *std,char *num)
{
	int i;
	STU a={"",9999,99,99};
	for(i=0;i<=N;i++)
/**********FILL**********/
		if(strcmp(【2】,num)==0)
/**********FILL**********/
			return (【3】);
	return a;
}
int main()
{
	STU std[N]={{"11111",1984,2,15},{"22222",1983,9,21},{"33333",1984,9,1},{"44444",1983,7,15},
{"55555",1984,9,28},{"666666",1983,11,14},{"77777",1983,6,22},{"88888",1984,8,18}};
	STU p;
	char n[10]="666666";
	p=fun(std,n);
	if(p.num[0]==0)
	{
		printf("\nNot found!\n");
	}
	else
	{
		printf("\nSucceed!\n");
		printf("%s   %d-%d-%d\n",p.num,p.year,p.month,p.day);
	}
return 0;
}

```

```c
【空 1 】	错误
【学生答案】
[1]      fun(STU *std,char *num)
【参考答案】
STU fun(STU *std,char *num)

============================================================
【空 2 】	错误
【学生答案】
if(strcmp(?2?,num)==0)
【参考答案】
std[i].num

============================================================
【空 3 】	错误
【学生答案】
return (?3?);
【参考答案】
std[i]

============================================================

```





#### 8.3

```c
/*请补充函数fun,该函数的功能是:建立一个带头结点的单向链表并输出到文件"out70.dat"和屏幕上,
各结点的值为对应的下标,链表的结点数及输出的文件名作为参数传入。注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的横线上填入所编写的若干表达式或语句。
试题程序: */
#include <stdio.h>
#include <stdlib.h>
typedef struct ss
{
	 int data;
	 struct ss *next;
}NODE;
void fun(int n,char*filename)
{
	 NODE *h,*p,*s;
	 FILE *pf;
	 int i;
	 h=p=(NODE *)malloc(sizeof(NODE));
	 h->data=0;
	 for(i=1;i<n;i++)
	 {
		s=(NODE *)malloc (sizeof (NODE));
/**********FILL**********/
		s->data=【1】;
/**********FILL**********/
		【2】;
/**********FILL**********/
		p=【3】;
	 }
	 p->next=NULL;
	 if((pf=fopen(filename,"w"))==NULL)
	 {
		printf("Can not open out98.dat!");
		exit(0);
	 }
	 p=h;
	 fprintf(pf,"\n***THE LIST***\n");
	 printf("\n***THE LIST***\n");
	 while(p)
	 {
		fprintf(pf,"%3d",p->data);
		printf("%3d",p->data);
		if(p->next!=NULL)
		{
			fprintf(pf,"->");
			printf("->");
		}
		p=p->next;
	 }
	 fprintf(pf,"\n");
	 printf("\n");
	 fclose(pf);
	 p=h;
	 while(p)
	 {
		s=p;
		p=p->next;
		free(s);
	 }
}
int main()
{
	 char *filename="out98.dat";
	 int n;
	 printf("\nInput n:");
	 scanf("%d",&n);
	 fun(n,filename);
return 0;
}

```

```c
【空 1 】	错误
【学生答案】
s->data=?1?;
【参考答案】
i

============================================================
【空 2 】	错误
【学生答案】
?2?;
【参考答案】
p->next=s;

============================================================
【空 3 】	错误
【学生答案】
p=?3?;
【参考答案】
p->next
p=s

============================================================

```



#### 8.4

```c
/*已知学生的记录由学号和学习成绩构成,N名学生的数据已存入a结构体中,给定程序的功能是找出成绩最低的学生记录,
通过形参返回主函数。注意:部分源程序给出如下。
请勿改动main函数和其他函数中的任何内容,仅在函数fun的横线上填入所编写的若干表达式或语句。 本题程序: */
#include <stdio.h>
#include <string.h>
#define N 10
typedef struct ss  /*定义结构体*/
{ char num[10]; 
  int s;
} STU;
void fun(STU a[], STU *s)
{
/**********FILL**********/
  【1】  h;
   int i;
   h=a[0];
   for(i=1;i<N;i++)
	if(a[i].s<h.s)
/**********FILL**********/
		【2】=a[i];
/**********FILL**********/
   *s=【3】;
}
int main()
{ 
STU a[N]={{ "A01",81},{ "A02",89},
{ "A03",66},{ "A04",87},{ "A05",77},
{ "A06",90},{ "A07",79},{ "A08",61},
{ "A09",80},{ "A10",71}},m;
  int i;
  printf("*****The original data*****");
  for(i=0;i<N;i++) 
     printf("No=%s Mark=%d\n", a[i].num,a[i].s);
  fun(a,&m);
printf("*****THE RESULT*****\n");
  printf("The lowest :%s, %d\n",m.num,m.s);
return 0;
}

```

```c
【空 1 】	错误
【学生答案】
?1?  h;
【参考答案】
STU

============================================================
【空 2 】	错误
【学生答案】
?2?=a[i];
【参考答案】
h

============================================================
【空 3 】	错误
【学生答案】
*s=?3?;
【参考答案】
h

============================================================

```



























