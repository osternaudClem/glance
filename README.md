## Installation

```bash
 bash -c '
  set -a
  source .env
  set +a
  envsubst < config/glance.yml.template | sed \'s/__INCLUDE__/$include/\' > config/glance.yml
  '
```
