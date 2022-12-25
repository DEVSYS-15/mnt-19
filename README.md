# Playbook для установки vector и clickhouse Lighthouse"

## Параметры
### all/vars.yml
1. clickhouse_http_port: "8123" 
1. clickhouse_listen_host_default:
     - "::1"
     - "0.0.0.0"
### Сlickhouse/vars.yml
1. ### clickhouse_packages
   ---
   - clickhouse-client
   - clickhouse-server
   - clickhouse-common-static
   ---
- список пакетов clickhouse
2. ### clickhouse_version: "22.2.2.1"
- версия clickhouse
### vector/vars.yml
1. ### vector_version: "1"
- версия резила vector
2. ### vector_release: "0.22.2"
- релиз vector
3. ### vector_url: "https://packages.timber.io/vector/{{ vector_release }}/vector-{{ vector_release }}-{{ vector_version }}.x86_64.rpm"
- ссыдка для скачивания vector
### Зависимости 
 - requirements.yml
### совметивмовсть 
- centos7

### совметивмовсть

- centos7
