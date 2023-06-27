# airflow-toy
## 초기 설정
### volume 디렉토리 생성, env파일 생성
```bash
mkdir -p ./dags ./logs ./plugins
echo -e "AIRFLOW_UID=$(id -u)" > .env
```
* ./dags - dag 파일 디렉토리  
* ./logs - task 실행 내역과 스케줄러 로그 디렉토리  
* ./config - 이 디렉토리에 커스텀 로그 파서 또는 airflow_local_settings.py을 만들어 클러스터 정책을 설정할 수 있다.  
* ./plugins - 커스텀 플러그인 디렉토리
### 포트 확인
Airflow: 8080  
PostgreSQL: 5432  
Redis: 6379
### airflow 기동
```bash
docker-compose up -d
```

