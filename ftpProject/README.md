# ʹ�ø��� 
   
#**����**  
server-> make;./server  ../conf/serverconf.ini      client-> make; ./client  127.0.0.1  2000     
Ĭ�� server ipΪ����ip,port=2000,�ӽ��̸���=5    

#**server��**   
���̳���Ӧclient ��¼��ע�ᡢ���ء��ϴ����ϵ����ء���־��¼����   
#**client��**  
����Ӧ��������ݰ����з���,�����˳��������
  
#**��¼��ע��**   
ע��: client salt��ֵ�������$6$.......��ʽ,crypt SHA-512����,���ɵõ���������,tcp���͸�server���浽mysql��    
��¼: server �ȷ����ѱ����salt��client,client�����ܺ���������뷢�͸�server,server��mysql���ݽ��бȶ�    
server��client�������Ӻ�,����while 1,ֻ��login�ɹ���break;   
login_password.sql �ļ�����login_password���ݿ��Լ���Ӧ�ı�ṹ   

#**������Ӧ**  
1.cd �����ӦĿ¼    
2.ls �г���ӦĿ¼�ļ�    
3.puts �������ļ��ϴ���������    
4.gets �ļ������ط������ļ�������    
5.remove ɾ�����������ļ�   
6.pwd ��ʾĿǰ����·��    
7.���������Ӧ    
8.�ͻ��˶Ͽ�,server �ӽ��̽����ȴ���һ������    

#**���ء��ϴ�**  
mmapӳ���ļ�,�õ�ӳ����ָ��,memcpy�����ݰ��в��Ϸ���      

#**�ϵ�����**  
���ش���ͬ���ļ�,�����д�С���͸�server,server mmapӳ��ʱƫ�ƶ�Ӧ��Сλ�ü���       

#**��־��¼**   
��¼�û�����¼ʱ�䡢�����������Ϣ��¼���浽�����ļ�       
server func.h ��¼��־�ľ���·��#define LogFile "/home/cuixuange/20170714/server/server.log" ��ֹcd �����ı��˹���·�����Բ����˾���·��  

#**��������**   
find ./ -name "*.c"|xargs wc -l   1700������
find /home/cuixuange/Linux_C_vacation -name *.c -or -name *.h -or -name *.cpp | xargs cat | grep -v ^$ | wc -l 