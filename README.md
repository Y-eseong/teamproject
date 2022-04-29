# miniProject
![premium-icon-vending-machine-2514680](https://user-images.githubusercontent.com/98035984/165918810-62f800eb-ca40-43db-8236-f95f280207fe.png)
# 디저트 자핀기
# mini project 주제
- 카페에 메뉴를 불러주는 자판기 

- mini project 에 대한 소개
  - 누구 이런 협업 어떤 수업 
  -

=
- mini project 가 가지고 있는 대략적인 기능 설명
## > typedef struct {
    char name[100];
    char contents[100];
    char weight[100];
    int price;
    int shipping;
    int coin; // 자판기에 넣은 돈
    }menu;


## CRUD
int ceateProduct(Product *p); // 제품을 추가하는 함수
void readProduct(Product *p); // 하나의 제품 출력 함수
int updateProduct(Product *p); // 제품을 수정하는 함수
int deleteProduct(Product *p); // 제품을 삭제하는 함수

void saveProduct(Product *p, int count); //데이터를 파일에 저장 하는 함수
int loadProduct(Product *p);// 저장된 데이터를 불러오는 함수

int selectMenu(); // 데이터를 다룰 때, 원하는 메뉴를 선택하는 함수
int selectDataNo(Product *p, int count); // 제품 번호를 불러오는 
int listProduct(Product *p, int count); // 전체 등록된 제품 리스트 출력
//검색기능 이름/가격/배송방법

void searchProductName(Product *p, int count); // 제품이름 검색
void searchProductPrice(Product *p, int count); // 제품가격 검색 
void searchProductShipping(Product *p, int count); // 배송방법 검색

void todayMenu(Product *p); // 랜덤으로 오늘의 추천 메뉴 알려주는 기능
//void inputCoin(Product *p); // 자판기 동전을 받는 기능
//int viewChange(); // 거스름돈 내역을 알려주는 기능

  - 기본 함수에 대한 설명 CRUUD, 파일로드 
  - void saveProduct(Product *p, int count); //데이터를 파일에 저장 하는 함수 이 함수를 이용하여 사용자가 선택한 메뉴를 저장한다.
  - int loadProduct(Product *p);// 저장된 데이터를 불러오는 함수 // 텍스트 파일을 영수증으로 사용하겠다 (recipt.txt)
  - 오늘의 메뉴를 추천 
    - 랜덤 함수를 이용하여 10가지 메뉴중에 하나를 추천 
  - 동전을 받고 거스름돈 계산 || 거스름돈을 다 사용할 경우 종료 || 중간에 종료 가능 
  
- 개발환경 및 언어
  -git 
  -vs code

- 팀소개 및 팀원이 맡은 역할
  - 역할 분담 
  - repo 소유자 : 김석원 /contributer : 김예성 
  - 어떤 함수 구현 하는지
  - 코드 관리 // 웹페이관리 
