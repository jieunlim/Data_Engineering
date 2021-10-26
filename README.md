
# Data-Engineering



#### 인터뷰질문1 (G*, 당근**)
    
    Sharding: Data를 분산해서 저장한다. 
    종류1) Horizontal partitioning ** permission과는 시스템에 따라 정의가 다를수 있음 
    종류2) Vertical partitioning
    Q1: Sharding의 경우 OLTP (Warehouse)가 아닌  OLAP (Production DB:mysql, oracle, postgressql) 중심  
    Q2: 샤딩이 제대로 분산되지 않고 쏠릴 때 어떻게 처리할 것인가? (** 추가조언: SQL 중요 특히 Window함수 연습 권장)
    
    ** 분산처리의 개념, 컨셉 인터뷰 질문 다수, 


#### 인터뷰질문2
    INSERT INTO를 잘 안씀, 정말 record가 작을때
    현업에서 한번에 몇백개씩 넣을때, INSERT INTO 호출, SQL만드는데 시간이 오래걸려서 BLUK INSERT (Redshift, snowflake, spark, hadoop)에서
    INSERT되는 Record- file(csc, json으로 만들어서)- cloud storage(s3) : redshift copy comment (5주차 예정)
    몇백만개 추가 20-30초 가능한 퍼포먼스 나옴

#### 인터뷰질문3 (G*)
    다양한 데이터 소스들에서 데이터를 불러 인프라를 빌딩해야한다. 어떻게 접근하겠는가? 그리고 어떻게 빌딩하겠는가?

