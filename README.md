# Bài 5: Test Coverage & Quality Enforcement (JaCoCo)

## Tích hợp JaCoCo

Đã cấu hình `jacoco-maven-plugin` trong `pom.xml` với 3 execution:
- `prepare-agent`: gắn agent để thu thập dữ liệu coverage.
- `report`: sinh báo cáo HTML trong `target/site/jacoco/`.
- `check`: kiểm tra coverage, yêu cầu **INSTRUCTION coverage >= 80%**.

## Quy tắc coverage

```xml
<limit>
    <counter>INSTRUCTION</counter>
    <value>COVEREDRATIO</value>
    <minimum>0.80</minimum>
</limit>