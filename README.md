                 +-------------+
                 |   Grafana   |
                 |   :3000     |
                 +------+------+
                        |
                        |
                 +------+------+
                 | Prometheus  |
                 |   :9090    |
                 +------+------+
                        |
              scrape /metrics
                        |
                 +------+------+
                 | Flask App   |
                 | book-backend|
                 |   :5001     |
                 +-------------+

User
 |
 :8080
 |
 nginx
 |
 +--- frontend
 |
 +--- backend API
