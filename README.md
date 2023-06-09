# aw05-zhaoxin
### 1. 在使用内存中的 h2 数据库时，应用程序的性能受到了限制。当同时有多个用户访问应用程序时，应用程序的响应时间明显增加，并且处理速度变慢。这是因为内存中的 h2 数据库只能处理有限数量的并发请求，而且无法进行水平扩展。因此，我们需要使用外部数据库（如MySQL或Redis）来处理会话数据和产品数据。
### 2. 在将应用程序部署到具有不同 CPU 的 Docker 容器中时，我们观察到了显著的性能差异。当将应用程序部署到具有更多 CPU 的容器中时，应用程序的响应时间更短，并且处理速度更快。这是因为容器可以分配更多的 CPU 资源来处理请求，从而提高了应用程序的性能。
### 3. 在使用 haproxy 进行水平扩展时，我们观察到了应用程序的性能显著提高。haproxy 可以将请求分发到多个应用程序实例中，从而提高了系统的并发处理能力。我们还发现，haproxy 在处理高并发请求时表现出色，可以有效地缓解服务器压力。
### 4. 在将应用程序更改为 RESTful 风格后，我们观察到了一些性能提升。由于客户端负责保存购物车状态，因此应用程序可以无状态地处理请求，从而减少了服务器端的负担。我们还可以使用缓存技术来缓存来自京东的产品数据，以进一步提高应用程序的性能。
#### 综上所述，我们可以通过使用外部数据库、增加 CPU 资源、使用 haproxy 进行水平扩展、将应用程序更改为 RESTful 风格以及使用缓存技术等方式来提高网络 POS 系统的性能。
