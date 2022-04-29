1. 메소드 리턴,이름,파라미터 타입 작성.

```java
    public int getCount(List<Object> list){
        return 0;
    }
    //리턴 타입 :   int 
    //메소드 이름:  getCount
    //파라미터 타입 :    List<Object>
```

2. 메소드 리턴,이름,파라미터 타입 작성.

```java
    public void insertData(Map<String, Object> map){

    }
    //리턴 타입 :   X(없다)
    //메소드 이름:  insertData
    //파라미터 타입 :   Map<String, Object>
```

3. 메소드 리턴,이름,파라미터 타입 작성.

```java
    public List<Object> list insertData(String str){
        return null;
    }
    //리턴 타입 :   List<Object>
    //메소드 이름:  insertData
    //파라미터 타입 :   String
```

4. 오버라이딩(Overriding)과 오버로딩(Overloading)이 무엇인지 간략히 기술하시오.

+ 오버로딩 : 생성자 메소드 에서 파라미터값을 다르게 하는것으로 여러개 사용하는것.
+ 오버라이딩 : 상속 으로 메소드를 불러와 사용하는것(*재정의)

5. 추상클래스와 Interface(인터페이스)에 차이점을 간략히 기술하시오.

+ 추상클래스는 하나만 상속받을수 있다. + 오버라이딩 *강제성
+ 인터페이스는 "," 을통해 여러개를 상속받을수 있다. 

6. 상속에 대해 아는 내용을 간략히 기술하시오.

+ 부모클래스를 이어받아 수 or 메소드등 사용할수 있다. 단 부모는 자식을 사용할수 없다.

7. 생성자에 대해 아는 내용을 간략히 기술하시오.

+ 클래스를 받아 변수 or 메소드등을 사용하는것(*초기화)

8. 컬렉션에 대해 아는 내용을 간략히 서술하시오.

+ <>: 을통해 클래스를 이용하여 배열,중복제거배열등을 오브젝트에서 불러와 사용하는것.

9. 아래 코드를 보고 예상되는 결과는?

```java
    class A{

        public static int count;
        public int temp;

    }
    class B{

        main(){

            A a1 = new A();
            a1.count = 10;
            a1.temp = 20;

            A a2 = new A();
            a2.count = 20;
            a2.temp = 20;

            System.out.println(a1.count); // 답 :   10 (정답:20)[public static int count]
            System.out.println(a1.temp); // 답 :    20

            System.out.println(a2.count); // 답 :   30 (정답:20)[public static int count;]
            System.out.println(a2.temp); // 답 :    20
        }
    }

```

10. 아래 코드를 보고 예상되는 결과는?

```java
    class A{
        public int money;
    }
    class B{
        public A getInstance(){
            A a = new A();
            return a;
        }
    }
    class C{
        main(){
            B b = new B();
            A a = b.getInstance();
            a.money = 1000;
            a = b.getInstance();
            a.money = a.money + 1000;
            System.out.println(a.money); // 답 :    1000
        }
    }
```

11. getter, setter을 이용하지 않고 필드변수 값을 초기화 하는 방법을 아래 코드로 작성하시오.

```java
class A{
    private String name;
    private int age;

    public A(String name, int age){
        this.name = name;
        this.age = age;
    }

}
```
