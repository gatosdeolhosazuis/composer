# Composer
## erro 1
```
The "https://repo.packagist.org/p2/symfony/error-handler.json" file could not be downloaded: SSL: Handshake timed out
  Failed to enable crypto
  failed to open stream: operation failed
```
```
composer config --global disable-tls true
composer config --global secure-http false
```
Adicionar "secure-http": falso no arquivo composer.json
```
"config": {
    "secure-http": false
},
```
```
composer clear-cache
composer diagnose
```
