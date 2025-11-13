# Grafana_Dashboard
version de prueba de un servidor de grafana online

**Instrucciones rápidas**

- **Requisitos:** Docker y Docker Compose disponibles en el entorno. Codespaces normalmente ya los proporciona.
- **Iniciar servicios:** desde la raíz del repo ejecutar:

```bash
docker compose up -d
```

- Grafana quedará disponible en el puerto `3000` (usuario/clave por defecto vienen de `.env`).
- Prometheus quedará disponible en el puerto `9090`.
- InfluxDB quedará disponible en el puerto `8086` (base por defecto: `metrics`).

**Archivos añadidos**

- `docker-compose.yml`: arranca `prometheus` y `grafana`.
- `prometheus/prometheus.yml`: config mínima de Prometheus.
- `grafana/provisioning/*`: provisioning de datasource y dashboards.
- `grafana/dashboards/sample-dashboard.json`: dashboard de ejemplo.
- `.env`: usuario/contraseña admin por defecto.

Si quieres que ajuste credenciales, añadir certificados, o añadir más dashboards/datasources, dime y lo hago.

