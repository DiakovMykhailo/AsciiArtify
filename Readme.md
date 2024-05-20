## Тестування скрипта як плагін kubectl`

Цей скрипт дозволяє отримати статистику використання ресурсів в кластері Kubernetes для певного простору імен та типу ресурсу.

### Параметри командного рядка:

1. Збережіть скрипт під іменем kubectl-kubeplugin (kubectl автоматично розпізнає плагіни, які починаються з kubectl-).

2. Зробіть скрипт виконуваним:

```bash
   chmod +x kubectl-kubeplugin
```

3. Перемістіть скрипт в директорію, яка є у вашому PATH, наприклад, /usr/local/bin:

```bash
sudo mv kubectl-kubeplugin /usr/local/bin/
```

4. Тепер ви можете викликати плагін за допомогою команди:
```bash
kubectl kubeplugin <namespace> <resource_type>
```
