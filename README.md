# manufactoring_data

Many global manufacturers around the world use Greenplum database.\
Therefore, we provide scripts and examples to build data based on the manufacturer's most commonly used cases.\
Various tests can be conducted through the sample table. 

To build the manufacturing sample data, follow these steps:

0.01_create_db.sh :  Create a test database \
0.02_create_role.sh : Create schema and role \
0.03_create_tbl.sh : Create test table \
0.04_create_func.sh : Create function using generation data  \
0.05_gen_code.sh : Generation Metadata \
0.06_gen_data.sh : Creating historical data ex)sensor data \
0.07_gen_array.sh : Serialize the generated data(0.06_gen_data.sh) into a table through an array and build it into a separate new table \
0.08_add_index.sh : Create index \
0.09_table_analyze.sh : Rebuild table analyze information \
0.10_table_size.sh : Table Size Comparison (General Table & arrayed Table) 
0.11_table_cnt.sh : Compare row count of sample data 
crt_function.sql : Create function file used in 0.04_create_func.sh 

The purpose of this data construction is to build data to compare query performance and the efficiency of system resource usage based on the difference in management between normal and arrayed tables with the same data. \
\
\
\
전세계 많은 글로벌 제조회사들은 Greenplum 을 사용하고 있습니다.\
제조사에서 많이 사용하는 사례를 기반으로 데이터를 구축하는 스크립트 및 예제를 제공합니다.\
해당 샘플 테이블을 통하여 다양한 테스트를 진행할 수 있습니다.

제조 샘플 데이터를 구축하는 순서는 다음과 같습니다.

0.01_create_db.sh :  새로운 데이터 베이스 생성 \
0.02_create_role.sh : 스키마 및 롤 생성 \
0.03_create_tbl.sh : 생산라인 테스트 테이블 생성 \
0.04_create_func.sh : 테스트 데이터 생성하는 Function 생성 \
0.05_gen_code.sh :  코드(메타)성 데이터 생성 \
0.06_gen_data.sh : : history성 데이터 생성 ex)sensor data \
0.07_gen_array.sh : 생성된 데이터를 array를 통하여 테이블 직렬화하여 별도 새로운 테이블로 구축 \
0.08_add_index.sh : 인덱스 생성\
0.09_table_analyze.sh : 테이블 통계 재생성\
0.10_table_size.sh : 테이블 사이즈 비교 ( 일반 테이블 & 직렬화 테이블 ) \
0.11_table_cnt.sh : 테이블 데이터 row 비교 \
crt_function.sql : 0.04_create_func.sh 에서 사용되는 create function 구문의 파일 

본 데이터 구축의 목적은 동일한 데이터를 가진 보통의 테이블과 Array화 된 테이블의 모델링의 차이에 따라 조회 성능과 시스템 리소스 사용의 효율성에 대해 비교하기 위해 데이터를 구축합니다.

데이터 구축이 완료되었다면 다음 링크를 통하여 성능 테스트를 진행해 보도록 합니다.




