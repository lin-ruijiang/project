#include<stdio.h>
int iLen_nax,iPos_max;//最长单词的起始位置
void tongji(char str[]}
{
    int i=0
    int iLen_each,iPos_each;
    char cFlag=1;
    char  ch;
    while(ch=str[i])
 {
  if(ch>='A'&&ch<='Z'||ch<'a'&&ch<='z')
{
 if(cFlag)
{
               cFlag=0;
                 iLen_each=0;
                 iPos_each=i;
        }
       iLen_each++
       }
else
{
           cFlag=1;
           if(iLen_each>iLen_max)
{
          iLen_max=iLen_each;
           iPos_max=iPos_each;
      }
   }
i++;
   }
if(iLen_each>iLen_max)
{
         iLen_max=iLen_each;
         iPos_max=iPos_each;
           }
     }
void main()
{
   char ch[1000];
   while（1）
{
       iLen_max=0；
       iPox_max=0;
       puts("请输入一行字母")
       gets(ch);
       tongji(ch);
       printf("最长单词的长度为:%d\n起始位置为;%d\n",iLen_max,iPos_max);
  }
system("pause");