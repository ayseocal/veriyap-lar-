# veriyapilari


include<stdio.h>
include<conio.h>
		int toplama(){
			int a=10, b=15;
	printf("islem turunu giriniz // + , - , * , / ");
	char islemturu;
	islemturu=getchar();
	int t,c,ca,bo;
	int *sonuc1,*sonuc2,*sonuc3,*sonuc4;
	t=a+b;
	c=a-b;
	ca=a*b;
	bo=a/b;

	sonuc1=&t;
	sonuc2=&c;
	sonuc3=&ca;
	sonuc4=&bo;

	printf("\n");
	switch (islemturu){
	case '+' :
		printf(" sayilarin toplami : %d ",*sonuc1);
		break;
	case '-' :
		printf(" sayilarin cikarimi : %d ",*sonuc2);
		break;
	case '*': 
		printf(" sayilarin carpimi  : %d ",*sonuc3);
		break;
	case '/' :
		printf("sayilarin bolumu :  %d ",*sonuc4);
		break;
		 default:
          printf("islem turunu girmediniz yada basmadiniz\n");
	}
	/*switch (islemturu){
	case '+' :
		printf(" sayilarin toplami : %d ",t);
		break;
	case '-' :
		printf(" sayilarin cikarimi : %d ",c);
		break;
	case '*': 
		printf(" sayilarin carpimi  : %d ",ca);
		break;
	case '/' :
		printf("sayilarin bolumu :  %d ",bo);
		break;
		 default:
          printf("islem turunu girmediniz ye basmadiniz\n");
	}*/
	return 0;
		}
		
	void main(){
		toplama();
		getch();
	}
		
