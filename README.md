  --Run sv_client.c and sv_server.c--

Mở 2 terminal chạy song song:

  --Terminal thứ nhất chạy:--
gcc sv_server.c -o sv_server
  
./sv_server

  --Terminal thứ hai chạy:--
  
gcc sv_client.c -o sv_client
./sv_client 127.0.0.1 9000

  --Run tcp_client.c and tcp_server.c--

Mở 2 terminal chạy song song:--

  --Terminal thứ nhất chạy:--

gcc tcp_server.c -o tcp_server
./tcp_server 9000 ./txt/hello.txt ./txt/log_tcp_server.txt

  --Terminal thứ hai chạy:--

gcc tcp_client.c -o tcp_client
./tcp_client 127.0.0.1 9000
