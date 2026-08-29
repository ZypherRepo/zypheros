# ZypherOS — Paketquelle 2.x

Erzeugt von `ota/publish-apt.sh`. Dieser Zweig wird bei jeder Veröffentlichung
**neu erzeugt**, hat also bewusst keine Historie.

## Einrichten

```sh
curl -fsSL https://raw.githubusercontent.com/ZypherRepo/zypheros/repo-v2/zypheros-archive-keyring.asc \
  | sudo gpg --dearmor -o /usr/share/keyrings/zypheros.gpg

echo "deb [signed-by=/usr/share/keyrings/zypheros.gpg] \
https://raw.githubusercontent.com/ZypherRepo/zypheros/repo-v2 stable main" \
  | sudo tee /etc/apt/sources.list.d/zypheros.list
```
