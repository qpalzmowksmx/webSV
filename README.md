# webSV

사용자, 항공편, 예약 관리 기능을 가진 다중 도메인 기반 웹 애플리케이션 개발
Spring Boot, JPA, MySQL, Thymeleaf, JSP/HTML, Gradle 등 사용
계층 분리 설계(Controller, Service, DAO, DTO)를 통해 유지보수성과 확장성 확보
예외 처리(GlobalExceptionHandler) 및 커스텀 예외 클래스 작성
테스트 코드(@SpringBootTest) 및 Docker 기반 배포 준비 파일 포함
실제 배포를 위한 Dockerfile, appspec.json 등 CI/CD 고려

AWS-Elastic Beanstalk 기반으로 서버리스 및 안전성 비용절감 구현

DB==> mysql-master-slave
2 region 1master/2slave

orchestrator

AWS EC2 서버에 MySQL 데이터베이스 운영 환경 구축
Prometheus와 Node Exporter를 이용해 데이터베이스 상태 모니터링 지표 수집
Grafana 대시보드 구성으로 지속적인 상태 시각화 및 가시성 확보
이상 징후 발생 시 경보(AlertManager) 발신 → Slack 연동을 통한 실시간 알림 처리
사용 기술: AWS EC2, MySQL, Prometheus, Node Exporter, Grafana, Slack Webhook
Linux 기반 시스템 설정 (포트 포워딩, 방화벽, 사용자 권한 제어 포함)
실시간 상태 지표 추적 (쿼리 수, CPU/메모리 사용량, 연결 수 등)
기술 포인트: 오픈소스 모니터링 도구 구성 및 Slack과의 경고 자동화 파이프라인 구축
Docker 환경에서도 동일한 구성이 가능하도록 컨테이너 기반 실습도 병행

with
https://github.com/qpalzmowksmx/Final-EC2
