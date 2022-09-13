# Java_0913-new-  
  
  
  
참조변수 - 객체!를 힙이라는 영역에 저장.참조변수는 주소를 가리킴. '.length'에서 .는 참조한다는 내용  
원시변수 - 실제값이 저장공간에 들어감  
  
  
소스는 하드디스크에 저장(설계도)-실행하는법은 컨트롤에프 십일을 눌러야 한줄한줄 처리가 됨.하드 디스크 소스를 시피유가 처리하는것이다 
램은 저장공간 - 씨피유가 처리하기에 필요한것(선언문에 따른 변수등)을 저장(공간을 할당함) 
씨피유는 모든 처리를 담당(공사업체)
  
  
package Tr;  
  
public class Day04 {  
	/*  
	 * 1.참조변수와 원시변수 구분  
	 * 데이터와 주소값  
	 * 선언문은 저장공간 확보한다는 뜻(변수를 이용해서)  
	 * <추가>연산자***  
	 * 2.조건문,반복문 이해 및 작성  
	 * 3.String 객체 배열에 저장하기  
	 * 4.1차원 배열에 값 저장하고 출력하기  
	 * 행만 있는것이 일차원 .행열 둘다 이차원.   
	 * 5.메서드 charAt()활용하여 특수문사 찾아내기  
	 * 	객체는 전역변수와(클래스 영역 전체에서 사용하는 변수) 메서드의 기능을 정의하고 있다.  
	 * 	객체는 클래스로 정의한다. 다시말해 하나의 클래스가 하나의 객체이다..?    
	 *  클래스는 자바 프로그램에서 원시 소스임.실행중인 프로그램이 아님 꼭 기억  
	 * 	객체는 개발자가 정의한 자료형이다.    
	 *   
	 * 전역변수:데이터를 저장하기위한 기억공간 ,원시변수와 참조변수를 구분하여 공부  
	 * 메서드 : 객체가 제공하는 기능이다.메서드는 어떤 기능을 가진 메서드인가?  
	 * 			매개변수 : ㅁㅔ서드를 호출할떼 넘겨주는 값(파라미터)  
	 * 			리턴타입 : 메서드가 실행한 후 호출부로 넘겨주는 값  
	 * 			리턴값 : 메ㅐ서드가 실행 한 후 호출부로 념겨주는 실제 데이터.  
	 * 	   
	 * 	고객을 객체로 정의해봐라 ..    
	 * 		정의: 아이디,비번, 기능: 아이디가 몇글자인지 알려주는 기능,비번에 특수 문자 있는지 등등    
	 * 		만약 위와같이 고객을 정의했다면 , 이 고객은 이름이라는 기능은 없다고 분석하면 됩니다.    
	 *   
	 * 		고객이라는 객체가 있고  
	 * 		매니저라는 객체가 있다.  
	 * 		매니저는 고객을 관리합니다.(관리의 범위는 가입 수정 탈퇴)  
	 *		매니저가 신규고객을 등록.아이디는 8글자로 사용.  
	 *		그럼 글자 체크하는 기능은 고객,매니저 둘중 어디에?  
	 *		답은 아무나 상관 없음 ->결정은 개발자가 함.   
	 */
```
		public static void main(String[] args) {
			
		
		String a = "abc";
		int aa =10;
		char b = 30;
		
		String[] c = new String[10];
		for(int i=0; i <c.length; i++) {
			c[i] = "human";
		} //저장하기
		
		System.out.println("-------------------");
		
		for(int i=0; i <c.length; i++) {
			System.out.println(c[i]); 
		} //출력하기
		
		String name = "human!ec";
		System.out.println(name.charAt(1));
		//System.out.println(name.);
		
		//선언문을 통해 String 타입의 객체를 만들고 주소값을 네임 변수가 저장
		//네임 변수가 참조하는 대상은 String 이라는 타입의 객체
		//자바에서 String 차입의 객체에게 정의된 기능(메서드)과 자원(전역변수)을 
		//네임변수가 참조하여 사용이 가능하다
		//개발자가 객체를 정의 하고 이 객체를 클래스로 작성하고 ,자바에서 제공하는 타입을 
		//활용하여 목적에 맞게 프로그램을 개발하는것이 주된 목적이다.
		
		String k = "동해 물과 백두산이";
		String kw = "두산";
		
		//charAtr()사용시 2중포문 사용해야함 -> indexOf(지정된 문자열이 처음나오는 인덱스 반환)
		System.out.println(k.indexOf(kw)+"----------");
		if(k.indexOf(k) != -1) {
			System.out.println("욕하지마 욕이 포함되어있네");
		}
		
		if(k.contains(kw)) {
			System.out.println("욕하지마 욕이 포함되었네2");
		}
		
		
		for(int i=0; i <name.length(); i++) {
			System.out.println(name.charAt(i));
		}
		
		for(int i=0; i<name.length(); i++) {
			if(name.charAt(i)!='!') {
				System.out.println(name.charAt(i)+"-------------");
			}
		}
	}
}
```
  
1차원 배열  
열로만 구성되어있음  
  
  
2차원 배열  
행과 열로 구성되어있음 (테이블 구조)  
  
  ![배열2](https://user-images.githubusercontent.com/80766275/189798881-98a51b72-dd6f-433e-bf1c-fe31d1424b86.PNG)
  
  
이차원 배열에 값을 넣는것은 이중포문 별찍기와 똑같다.  
```
int ccnt =1; //값 저장하는 변수  
int[][] c = new int[4][8];  
  
for(int i=0; i<4; i++){ //i는 행을 의미
  for(int j=0; i<8; j++){
    c[i][j] = ccnt; ccnt++; 
 }
}  //입력부
```
  
배열에 그냥 넣기  
  
  
```  
package Tr;

public class Day04_1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int ccnt = 1;
		int[][] c = new int [4][8];
		
		for(int i=0; i<4; i++) {
			for(int j=0; j<8; j++) {
				c[i][j] =ccnt; ccnt++;
			}
		} //입력부
		for(int i = 0; i<4; i++) {
			for(int j=0;j<8;j++) {
				System.out.print(c[i][j]+"\t");
			}
			System.out.println();
		}//출력부
		
		int[][] d = {
				{10,20,30,40,50},
				{10,20,30,40,50},
				{10,20,30,40,50},
				{10,20,30,40,50}
	
		}; //초기값 수기로 넣기 
		
		
	}

}
```  
  
  
  
  
  
  
  ![배열거꾸로 넣기](https://user-images.githubusercontent.com/80766275/189801889-dbad7a25-fae0-400e-b628-04ea188470db.PNG)
하는 방법  
  
  
```  
package Tr;
public class Test {

   public static void main(String[] args) {
      // TODO Auto-generated method stub
      
      
      int ccnt=1;
      int [][]c =new int [4][5];
            
      for(int i=0;i<4;i++) {
         for(int j=4;j>=0;j--) {//j=4,3,2,1,0
                  c[i][j]=ccnt;
                  ccnt++;
               }
            }
      for(int i=0;i<4;i++) {
         for(int j=0;j<5;j++) {
            System.out.print(c[i][j]+"\t");
         }
         System.out.println();
      }
   }

}
```  
  
위의 예제 두가지는 마스터 해야함  

  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
