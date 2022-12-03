### Component 설명
* api
    * REST API Server
    * Swagger를 통한 API 명세 제공
    * Core / Domain / Infrastructure를 활용하여 Web 서비스 제공
    * MVC의 Controller 역할
    * Request / Response 관리 및 Filter / Interceptor / Handler 기능 구현
* batch
    * Batch Module
    * 배치 작업이 필요할 시 Core / Domain / Infrastructure를 활용하여 구현
* client
    * 타 도메인에 Rest API Library 제공 용도
    * Feign Client 등을 활용
* core
    * Business Logic은 아니지만 프로젝트 전반에서 공통적으로 사용되는 모듈
    * Exception, Enum, DTO, Utility 성 모듈등
* domain
    * Business Logic
    * Service, Repository, Domain(Entity, Aggregate, Aggregate Root)
* infrastructure
    * 외부 시스템과의 연동을 위한 모듈
    * Networking Module
    * JPA / MyBatis 등의 DB Persistent Framework 연동 모듈
    * Kafka / RabbitMQ 등의 MQ 연동 모듈
    * Redis / Elasticache 등의 No-SQL 연동 모듈