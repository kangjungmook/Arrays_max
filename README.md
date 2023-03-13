# 자바 배열 최대값 구하기

* 배열 선언하기. int[] intarray= new int[] {1,2,3,4,5};
* 최댓값을 담을 변수 선언하고 배열의 인덱스 0 값 참조하기. int max = intarray[0];
* for문 if문 활용해 최댓값 찾기.
* 최댓값 출력하기.

## for 문과 if 문 을 이용하여 최대값 구하기
```java
    Scanner sc = new Scanner(System.in);

        System.out.println("사람의 수를 입력하세요");
        int num = sc.nextInt();
```
* 스캐너로 정수 받아오기
 ```java
   int arr[] = new int[num];
        for (int i = 0; i <= num - 1; i++) {
            System.out.println("height[" + i + "]");
            arr[i] = sc.nextInt();
        }
 ```
 * 배열을 선언하고 스캐너로 불러 온 정수 출력하여 사람의 수가 몇명인지 알기
  배열의 개수 만큼 성적을 넣기
 ```java
       for (int i = 1; i < arr.length; i++) {
            if (arr[i] > max) {
                max = arr[i];
            }
        }
        System.out.println("최대값은"+max+"입니다");
    }
}
 ```
 * 성적을 넣은걸 for문을 이용하요 계속 if 랑 비교 하여 max 보다 arr[i]에 계속 반복하면
 가장 큰애가 max에 저장 따라서 max 값을 출력하면 배열중에서 가장 큰값을 출력
