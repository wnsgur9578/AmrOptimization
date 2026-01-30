<img width="1122" height="485" alt="image" src="https://github.com/user-attachments/assets/eec085e3-1df7-4c72-b97c-c35033d66afc" />

# AmrOptimization
- 물류를 배달하는 AMR 시뮬레이션을 진행
- 시뮬레이션의 TotalTardiness(총 지연시간) 최소화가 목표

# 역할
- 베이스 라인을 기반으로 프로젝트 방향성 핸들링
- AMR 개수 파트 담당
- Dispatching rule 파트 담당

# 요약

- 문제 정의
    - 한 시뮬레이션의 비용과 시간을 최소화

- 데이터 생성
    - 유전 알고리즘을 통해서 work center, 물류 센터 등의 학습에 필요한 데이터 생성
 
- 최소화 방법
    - 시간을 최소화하기 위해 Dispatching Rule과 머신러닝을 활용
        - Dispatching Rule로는 FIFO, EDD, LST, LPT, SPT를 적용
        - 머신러닝 기법으로는 랜덤 포레스트, XGBoost, DNN을 사용
    - 비용 최소화를 위해 시뮬레이션당 최소 비용 함수를 생성
        - AMR 수를 변경하며 비교한 결과, 3개일 때 가장 낮은 비용 달성
  
# 결론
 - FIFO, EDD, 그리고 XGBoost가 가장 효과적인 결과를 보였음
 

